.. _External Grader:

###########################
外部打分
###########################

.. _External Grader Overview:

*******************
概览
*******************

外部打分是一项接收学习者对一个问题的反应，处理这些反应并返回反馈和对问题的打分到edX平台的服务。你可以分别从edX平台建立和配置外部打分。

请看以下部分以获取更多信息：

* :ref:`外部打分示例`
* :ref:`外部打分和XQueue`
* :ref:`XQueue接口`
* :ref:`建立外部打分`
* :ref:`创建一个代码回答问题`

.. _External Grader Example:

***************************
外部打分示例
***************************

外部打分对学习者被要求提交复杂的代码的软件编程课程特别有用。打分可以运行你定义的测试，然后把结果返回给学习者。

例如，你定义一个要求学习者提交Python代码的问题，并创建一个测试集，外部打分可以运行来核实提交。当学习者输入Python代码并选择 **检查**，代码就会被送到打分来测试。如果代码通过了全部测试，打分就返回得分以及一个提示解答正确的字符串。

.. image:: ../../../shared/building_and_running_chapters/Images/external-grader-correct.png
 :alt: Image of a learner's view of a programming problem that uses an external grader, with a correct result.
 :width: 600

外部打分能返回带结果的字符串，通过选择 **查看全部输出** 学习者可以查看。当解答不正确且你想返回关于测试失败的信息时，这是特别有用的。例如：

.. image:: ../../../shared/building_and_running_chapters/Images/external-grader-incorrect.png
 :alt: Image of a learner's view of a programming problem that uses an external grader, with an incorrect result 

.. _External Graders and XQueue:

**************************************
外部打分和XQueue
**************************************

edX平台通过XQueue与你的外部打分进行通信。XQueue提供学习者对打分的输入，然后接收从打分返回的输出并返回给学习者。

提交被收集在XQueue中，它们保留在其中直到打分检索或拉取下一个提交。

外部打分在常规时间间隔通过一个有REST特性的接口对XQueue进行轮询。当外部打分检索一个提交，它就运行测试，然后打结果推回到XQueue中，同样是通过具有REST特性的接口。XQueue然后把结果传递到edX学习管理系统。

使用拉取模式的外部打分的示例代码，请看 `Stanford-
Online repository xqueue_pull_ref <https://github.com/Stanford-
Online/xqueue_pull_ref>`_.

============================
外部打分工作流程
============================

接下来的步骤描述了外部打分评估一个问题的全部过程

#. 学习者输入对问题的代码或上传文件，然后选择 **检查**.

#. 外部打分从XQueue拉取代码

#. 外部打分运行你针对代码创建的测试

#. 外部打分在字符串中返回提交的得分和其他的结果，到XQueue

#. XQueue传递结果到edX学习管理系统

#. 学习者看到问题结果和得分

==================
XQueue名称
==================

你的课程会使用一个特定的XQueue名称。当你在Studio中创建问题时使用这个名称。

使用外部打分的edX合伙人应该使用基础URL
``https://xqueue.edx.org`` 作为XQueue名称。

如果你是一位edX合伙人，联系你的edX程序管理员以获取更多信息。因为edX为不同的课程群集许多XQueue，如果在你的课程中必需使用特定的XQueue名称，如 :ref:`创建一个代码回答问题` 中所描述的。

.. _The XQueue Interface:

**************************************
XQueue接口
**************************************

从XQueue发送到打分的学习者的提交，以及从打分发送到XQueue的结果都是JSON对象，描述如下：

.. note:: 
  XQueue不发送学习者的ID到外部打分，你的打分不能访问ID或与提交关联的学习者的ID。

XQueue接口的代码，请查看文件 `urls.py in the edX XQueue
repository <https://github.com/edx/xqueue/blob/master/queue/urls.py>`_.

======================================================
外部打分的输入
======================================================

打分作为JSON对象接收提交，其有关键：

* **学生回答** ：一个字符串，包含学习者的提交代码。这个字符串来自学习者在edX学习管理系统的输入或学习者上传的文件。

* **打分负荷** ：一个可选的字符串，用来指定你在何时创建了问题。更多信息，请看 :ref:`创建一个代码回答问题` 部分

例如::

 {
   "xqueue_body":
   "{
     "student_response": "def double(x):\n return 2*x\n", 
     "grader_payload": "problem_2"
    }"
 }

======================================================
外部打分结果
======================================================

在运行测试和记录提交的结果后，打分必需通过传递JSON回复来返回信息。JSON字符串包含一个值，该值表明无论提交是否正确，以及得分和测试产生的任何消息。

在接下来的例子中，学习者的提交是正确的，得分为1，测试产生一个简短的消息::

 { 
  "correct": true, 
  "score": 1, 
  "msg": "<p>The code passed all tests.</p>" 
 }

.. _Building an External Grader:

****************************
建立外部打分
****************************

课程教员，而不是edX，负责建立和配置外部打分。

除了创建针对你在课程中使用的问题的测试外，当建立外部打分，还有四个方面你必须作规划：

* :ref:`扩展`
* :ref:`安全`
* :ref:`可靠性和恢复`
* :ref:`测试`

.. _Scale:

==================
扩展
==================

你的外部打分必须能扩展足以支持你的课程中的学习者人数。

记住提交可能会突发，而不是一个均匀的流量。例如，你应该预期到在考试到期之前几小时负载个比平均大很多。所以，你应该确定外部打分能在短时间内处理大多数学习者的提交。

.. _Security:

==================
安全
==================

学习者提交的代码在你负责的服务器上直接执行。学习者可能提交恶意代码。你的系统必须能免受其害，保证外部打分只运行与问题相关的代码。你如何实现这些保护取决于你使用的编程语言和你的应用构架。你必须确保恶意代码不会损害你的服务器。

.. _Reliability and Recovery:

==============================
可靠性和恢复
==============================

在你的课程开始之后，许多学习者会在任何时候提交代码，并期望马上能看到结果。如果你的外部打分易于失败或有不可预期的延迟，学习者的体验会变糟糕。

所以，你必须确保你的打分有高可用性，能够从错误中恢复。在你的课程开始之前，你必须做一个计划使得在打分失败后，立刻通知负责操作你的打分和edX的团队。与edX合作，你必须开发一个过程来识别失败的原因，原因可能来自edX，或你的打分。

联系edX程序管理员以获取更多信息。

如果你知道打分会在维护的时期不可用，你应该 :ref:`添加课程更新 <Add a Course Update>`.

.. _Testing:

==================
测试
==================

你应该在你的课程开始之前完全地测试你的打分。保证测试不正确的代码和正确的代码来确保打分会产生合适的得分和消息。

.. _Create a Code Response Problem:

********************************
创建代码回答问题
********************************

你在edX Studio中通过添加一个普通空白问题，然后编辑在 :ref:`高级编辑器` 中的XML问题定义来创建代码回答问题。

请参照 :ref:`与问题组件协作` 来获取更多信息。

接下来是使用了外部打分的问题的XML定义的一个基本例子::

 <problem display_name="Problem 6">
    <text>
        <p>Write a program that prints "hello world".</p>
    </text>
    <coderesponse queuename="my_course_queue">
        <textbox rows="10" cols="80" mode="python" tabsize="4"/>
        <codeparam>
            <initial_display>
              # students please write your program here
              print ""
            </initial_display>
            <answer_display>
              print "hello world"
            </answer_display>
            <grader_payload>
            {"output": "hello world", "max_length": 2}
            </grader_payload>
        </codeparam>
    </coderesponse>
 </problem>

注意接下来关于XML定义的细节

* **队列名称**： 具有 ``<coderesponse>`` 队列属性的元素的值映射到一个XQueue。合伙人应该联系他们的edX程序管理员获得更多信息。你必须使用这个确切的名称，使得问题与正确的XQueue通信。

  .. note:: 
    对于edX合伙人，打分必须访问的基URL是
    ``https://xqueue.edx.org``.

* **输入类型**：在这个例子中， ``<textbox>`` 元素指定了输入类型。当你看到 ``<textbox>`` 时，学习者在查看课程单元时在浏览器中输入代码。其他的你可以用来指定输入类型的元素是 ``<filesubmission>``，其使得在单元中学习者能上传和提交代码文件。

* **<打分负荷>**：你可以使用 ``<grader_payload>`` 元素来发送信息到外部打分，以JSON对象的格式。例如，你可以使用 ``<grader_payload>`` 告诉打分为这个问题运行哪个测试。

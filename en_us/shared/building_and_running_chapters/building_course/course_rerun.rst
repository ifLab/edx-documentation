.. _Rerun a Course:

###################
重开课程
###################

另一个在Studio中创建课程的方式是重开一门已有课程。
当您选择课程重开选项，大多数原有的课程内容将复制生成新课程。
原始的课程不会改变。

* :ref:`Data Duplicated When You Re-Run a Course`
* :ref:`Use Re-Run to Create a Course`
* :ref:`Update the New Course`

.. _Data Duplicated When You Re-Run a Course:

********************************************
重开课程的数据复制
********************************************

.. list-table::
   :widths: 45 45
   :header-rows: 1

   * - 内容类型
     - 复制到新课程？
   * - 课程开始日期
     - 否。设置为2030年1月1日零点（UTC）
   * - 所有其他课程日期
     - 是。您必须更新所有发布日期和截止日期。
   * - 课程结构（章节、小节、单元）和状态（公开、隐藏）

     - 是。
   * - 独立问题和其他组件
     - 是。
   * - 已上传至课程的文件，包括视频和课本
     - 是。
   * - 添加的页面
     - 是。 包括所有页面内容和已定义的页面顺序。
   * - 课程更新
     - 是。
   * - 高级设置
     - 是。
   * - 评分标准
     - 是。
   * - 学生注册信息
     - 否。
   * - 课程团队特权，包括管理员、论坛版主、贝塔测试员

     - 否。 只有创建新课程的用户可以访问
   * - 手动创建队列小组
     - 否。
   * - 学生答案、进度和成绩数据
     - 否。
   * - 证书
     - 否。
   * - 论坛发帖、回复、评论和其他数据
     - 否。
   * - 维基贡献
     - 否。

重开课程之后，对原有课程的修改和对重开课程的修改是相互独立的。
对其中一门课程的修改不会影响到另一门课程。
所以，在重开课程之前，您应该确保原有课程内容尽量完善。

更多信息请参阅 :ref:`Use Re-Run to Create a Course` and :ref:`Update the New Course`.

.. _Use Re-Run to Create a Course:

********************************************
使用重开建立课程
********************************************

在重开课程之前，请完成以下步骤。

* 在 `edge.edx.org`_ 上的课程请确保您有在Studio的开课许可。

* 在 `edx.org`_ 上的课程，请联系您的项目经理。
  您的项目经理将使用重开特性创建新课程，然后与您一起完成 :ref:`update the new
  course<Update the New Course>` 中的步骤。

* 保证课程内容完整。创建新课程以后，您在原始课程上的改动将不会出现在新课程中。

要重开课程，您必须在Studio中有创建课程的许可，您必须是重开课程的教员。

按照以下步骤重开课程：

#. 登录Studio。面板中列出了您作为教员访问的课程。

#. 将光标移至列表中的每一行。每门课程上显示 **重开课程** 和 **在线查看** 选项。

  .. image:: ../../../shared/building_and_running_chapters/Images/Rerun_link.png
     :alt: A course listed on the dashboard with the Re-run Course and View
           Live options shown
     :width: 600

3. 找到您想重开的课程，选择 **重开课程** 。 **以当前课程创建重开课程** 页面开启，
   **课程名** 、 **组织** 和 **课程号** 栏中已经填入了默认值。

  .. image:: ../../../shared/building_and_running_chapters/Images/rerun_course_info.png
     :alt: The course creation page for a rerun, with the course name,
           organization, and course number supplied.
     :width: 600

4. 填入 **课程开启** 指明新课程何时启动。

   课程号、组织和课程开启，三个值用来创建新课程的URL。新课程的这三个值组合必须是唯一的。
   此外，名称、组织、编号和开启时间总字符数不能超过65.

5. 选择 **创建重开课程** 。 **我的课程** 面板开启，显示一条关于课程创建进程的消息。

  复制课程结构和内容需要几分钟的时间。程序进行时，您可以在Studio或学习管理系统，
  或者其他网页中进行其他工作。配置完成后，新课程将出现在Studio **我的课程** 面板。


.. _Update the New Course:

********************************************
更新新课程
********************************************

当您通过重开课程创建一门新课程时，您必须仔细查看新课程的设置和内容。
为了保证学生的良好学习体验，请确保在开课之前测试课程。
参阅 :ref:`Testing Your Course Content` 和
:ref:`Beta_Testing` 。

至少，您必须做出下列修改以准备发布新课程。

* 增加课程教员，包括论坛管理员、版主和社区助教。
  请参阅 :ref:`Add Course Team Members` 或 :ref:`Course_Staffing` 。

* 更新全课堂日期，包括课程起止日期和注册时间。
  请参阅 :ref:`Scheduling Your Course` 。

* 更改课程章节、小节和单元的发布日期。
  请参阅
  :ref:`Release Dates` 。

* 更改评分政策中的小节截止日期。
  请参阅
  :ref:`Set the Assignment Type and Due Date for a Subsection` 。

* 在Studio中删除或修改所有在 **课程更新** 页面中的帖子。
  请参阅 :ref:`Add
  a Course Update` 。

* 在 **文件与上传** 页面中查看文件。如果需要更新包含课程相关日期的文件，您必须完成以下步骤。

  1. 找到原文件来源。
  2. 在文件中修改课程相关日期。
  3. 上传修改后的文件。

  .. note:: 如果您在上传文件时使用原来的文件名，课程组件和讲义中的文件链接仍然有效。
   如果您更改了文件名，您必须更新所有链接。请参阅 :ref:`Add Course Handouts`
   or :ref:`Add a Link to a File`.

* 查看教员信息和其他课程总结页面的信息，并作相应更新。
  请参阅 :ref:`The Course About Page`.

* 为讨论主题发布初始帖和 “自我介绍” 帖。
  请参阅 :ref:`Discussions`.

* 添加原始维基文章。

您可以使用 :ref:`course checklists<Use the Course Checklist>` 来检查课程，
确保课程已经可以发布。您也可以查看 :ref:`Launch` 主题，其中有帮助您准备开启课程的工具和提示。

.. note::
  对新课程的修改不会影响原始课程。

.. _edge.edx.org: http://edge.edx.org
.. _edx.org: http://edx.org

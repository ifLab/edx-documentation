.. _Dropdown:

#####################
下拉问题
#####################

下拉问题让学生从下拉列表中显示的答案里选择一个答案。 不同于 :ref:`多项选择问题<Multiple
Choice>` 选择项是一直可见的， 下拉问题需要学习者点击下拉箭头才会显示选项。

.. image:: ../../../shared/building_and_running_chapters/Images/DropdownExample.png
 :alt: A problem component with 3 dropdown problems, 2 marked correct and 1
     incorrect

你可以使用edXInsights来查看汇总的学生学习能力数据以及评判已经提交的答案。 欲了解更多信息，请参阅 `Using edX Insights`_.

********************************
创建一个下拉问题
********************************

你可以在简单编辑器或者高级编辑器中创建下拉问题。 您可以在简单的编辑器创建题目，然后切换到高级编辑器用XML添加更多的配置选项。 但是你不能从高级编辑器切换回简单编辑器。 因此你要尽可能在开始使用高级编辑器之前完成对问题的排版工作。
 
.. _Use the Simple Editor to Create a Dropdown Problem:

========================================================================
使用简单编辑器来创建下拉问题
========================================================================

使用 :ref:`简单编辑器<Simple Editor>` 来创建下拉问题，遵循以下步骤：

#. 在你想创建问题的单元处，选择 **添加新的组建** 中的 **问题** 选项。
#. 在 **常用问题种类** 列表中选择 **下拉** 。 编辑器会添加一个示例下拉问题到该单位中。
#. 选择 **编辑** 。 简单编辑器打开。
#. 用自己的文本替换示例中的文本。
#. 写一段文本来描述你想让学生回答的问题，用两对尖括号将这段文本扩住 (``>>问题的具体内容<<``)。 这段文字就是这个问题的标签。
#. 将所有可能的答案都写在同一行，用逗号分割。
#. 选择所有答案选项， 然后在工具栏中选择选择 **下拉** 。 两组方括号 ([[ ]]) 会出现在答案选项的两边。
#. 在正确答案的两边用圆括号将其标记出来。
#. 选择解释文本然后选择工具栏中的 **说明** 来为该问题提供解释说明。 ``[解释说明的文本]`` 标记会出现在解释文本的起始位置和结束位置。 
#. 选择 **设置** 然后为该问题提供一个用来识别的 **显示名称** 。
#. 定义的问题的其他设置。 欲了解更多信息，请参阅
   :ref:`Problem Settings`.
#. 选择 **保存** 。

下面的文本是上面的示例问题在问题组件中所显示的内容。

::

    >>What type of data are the following?<<

    Age:
    [[Nominal, Discrete, (Continuous)]]
    Age, rounded to the nearest year:
    [[Nominal, (Discrete), Continuous]]
    Life stage - infant, child, and adult:
    [[(Nominal), Discrete, Continuous]]

========================================================================
使用高级编辑器来创建下拉问题
========================================================================

用高级编辑器来创建下拉问题需要以下步骤。

#. 按照 :ref:`简单编辑器<Use
   the Simple Editor to Create a Dropdown Problem>`. 中的步骤来创建题目。
#. 选择 **高级编辑器**，然后编辑XML来添加你想要的标记和属性。 下面是一个例子。

**题目的代码**:

.. code-block:: xml

  <problem>
  <p>
    <em>This exercise first appeared in HarvardX's PH207x Health in Numbers: Quantitative Methods in Clinical &amp; Public Health Research course, fall 2012.</em>
  </p>
  <p>What type of data are the following?</p>
  <p>Age:</p>
  <optionresponse>
    <optioninput options="('Nominal','Discrete','Continuous')" correct="Continuous" label="Age"/>
  </optionresponse>
  <p>Age, rounded to the nearest year:</p>
  <optionresponse>
    <optioninput options="('Nominal','Discrete','Continuous')" correct="Discrete" label="Age, rounded to the nearest year"/>
  </optionresponse>
  <p>Life stage - infant, child, and adult:</p>
  <optionresponse>
    <optioninput options="('Nominal','Discrete','Continuous')" correct="Nominal" label="Life stage"/>
  </optionresponse>
  </problem>

.. _Dropdown Problem XML:

************************
下拉问题的XML代码
************************

========
模板
========

.. code-block:: xml

  <problem>
  <p>Question text</p>
  <optionresponse>
    <optioninput options="('Option 1','Option 2','Option 3')" correct="Option 2" label="label text"/>
  </optionresponse>
    <solution>
      <div class="detailed-solution">
      <p>Explanation or Solution Header</p>
      <p>Explanation or solution text</p>
      </div>
    </solution>
  </problem>

.. code-block:: xml

  <problem>
  <p>Question text</p>
    <optionresponse>
     options="('A','B')"
      correct="A"/>
      label="label text"
    </optionresponse>
   
    <solution>
      <div class="detailed-solution">
      <p>Explanation or Solution Header</p>
      <p>Explanation or solution text</p>
      </div>
    </solution>
  </problem>

========
标记
========

* ``<optionresponse>`` (必须的): 表示这个问题是一个下拉问题。
* ``<optioninput>`` (必须的): 列出答案选项。

**标记:** ``<optionresponse>``

表示这个问题是一个下拉问题。

  属性

  (无)

  子标记

  ``<optioninput>``  

**标记:** ``<optioninput>``

列出答案选项。

  属性

  .. list-table::
     :widths: 20 80

     * - 属性
       - 描述
     * - 选项 (必须的)
       - 列出答案选项。 答案选项列表被圆括号括住，各个答案被单引号 (') 括住，并用逗号分隔各个答案 (,)。
     * - 正确性 (必须的)
       - 标示一个答案是否正确。 可以是"正确"或者"错误"。 只有一个 **正确性** 属性可以被设置成正确。
     * - 标签 (必须的)
       - 指定回复区的名字。
  
  子标记

  (无)



.. _Using edX Insights: http://edx.readthedocs.org/projects/edx-insights/en/latest/

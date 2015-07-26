.. _Checkbox:

##################
复选框问题
##################

在复选框问题中, 学习者从可能的答案列表中的选择一个或多个选项.为了正确回答问题,学习者必须选择所有正确的选项. 每个复选框问题必须有一个或多个正确选项.

.. image:: ../../../shared/building_and_running_chapters/Images/CheckboxExample.png
 :alt: A checkbox problem with four options, 2 of which are required for the
     correct answer

对于在你课程中的复选框问题,你可以使用edX Insights评估学习者成绩数据和检查提交过的答案. 更多相关信息,请查看： `Using edX Insights`_.

****************************
创建一个复选框问题
****************************

你可以使用简单编辑器或高级编辑器创建复选框问题.你可以在简单编辑器中设置一个问题，然后切换到高级编辑器来添加更多的XML中的配置选项.然而,你不能从高级编辑器切换回简单编辑器。因此,你可能会想要尽可能完全地确定问题的格式在你开始使用先进的编辑器之前。


.. _Use the Simple Editor to Create a Checkbox Problem:

======================================================
使用简单编译器创建复选框问题
======================================================

要使用 :ref:`简单编辑器<简单编辑器>` 创建一个复选框问题,
有以下的步骤.

#. 在你想要创建问题的单元里, 在 **添加新组件** 下方选择 **问题**.
#.  **常见问题类型**, 选择 **复选框**. 添加一个复选框问题到单元中.
#. 选择 **编辑**. 简单编辑器就打开了. 
#. 用你自己的问题文本替代样本问题文本.
#. 确定你想让学生回答的问题的文本描述,用双肩括号括住 (``>>问题<<``).这个问题文本是这个问题的访问标签。
#. 将每个答案选项放在单独的行中。
#. 选择你设置的答案选项, 然后在工具烂选择**复选框**.在每个选项的旁边就出现了一对括号.
#. 为了识别每个正确答案, 要在这个选项旁边的括号中间添加一个**x**.
#. 要提供一个说明, 选择说明文本然后从工具栏中选择**说明**. ``[说明]`` 出现在说明文本的前面和后面。
#. 选择 **设置**并为这个问题提供一个识别 **显示名称**.
#. 为这个问题定义额外的设置. 更多相关信息,请查看： :ref:`Problem Settings`.
#. 选择 **保存**.

For the example problem illustrated above, the following text displays in the
problem component.

.. code-block:: xml

    Learning about the benefits of preventative healthcare can be particularly 
    difficult. >>Check all of the reasons below why this may be the case.<<

    [x] A large amount of time passes between undertaking a preventative measure and seeing the result. 
    [ ] Non-immunized people will always fall sick. 
    [x] If others are immunized, fewer people will fall sick regardless of a particular individual's choice to get immunized or not. 
    [x] Trust in healthcare professionals and government officials is fragile. 

.. please do not line wrap this example:

    [explanation]
    People who are not immunized against a disease may still not fall sick from the disease. If someone is trying to learn whether or not preventative measures against the disease have any impact, he or she may see these people and conclude, since they have remained healthy despite not being immunized, that immunizations have no effect. Consequently, he or she would tend to believe that immunization (or other preventative measures) have fewer benefits than they actually do.
    [explanation]


========================================================================
Use the Advanced Editor to Edit a Checkbox Problem 
========================================================================

To use the :ref:`Advanced Editor<Advanced Editor>` to edit a checkbox
problem, follow these steps.

#. Follow the steps for creating the problem in the :ref:`Simple Editor<Use
   the Simple Editor to Create a Checkbox Problem>`.
#. Select **Advanced Editor**, and then edit the XML to add the tags and
   attributes you want. An example follows.

.. code-block:: xml

  <problem>
  <p>Learning about the benefits of preventative healthcare can be particularly difficult. Check all of the reasons below why this may be the case.</p>

  <choiceresponse>
    <checkboxgroup label="Check all of the reasons below why this may be the case">
      <choice correct="true"><text>A large amount of time passes between undertaking a preventative measure and seeing the result.</text></choice>
      <choice correct="false"><text>Non-immunized people will always fall sick.</text></choice>
      <choice correct="true"><text>If others are immunized, fewer people will fall sick regardless of a particular individual's choice to get immunized or not.</text></choice>
      <choice correct="true"><text>Trust in healthcare professionals and government officials is fragile.</text></choice>
    </checkboxgroup>
  </choiceresponse>

   <solution>
   <div class="detailed-solution">
   <p>Explanation</p>
   <p>People who are not immunized against a disease may still not fall sick from the disease. If someone is trying to learn whether or not preventative measures against the disease have any impact, he or she may see these people and conclude, since they have remained healthy despite not being immunized, that immunizations have no effect. Consequently, he or she would tend to believe that immunization (or other preventative measures) have fewer benefits than they actually do.</p>
   </div>
   </solution>
  </problem>

.. _Checkbox Problem XML:

****************************
Checkbox Problem XML 
****************************

============
Template
============

.. code-block:: xml

  <problem>
  <p>Question text</p>

  <choiceresponse>

  <checkboxgroup label="label text">
  <choice correct="false"><text>Answer option 1 (incorrect)</text></choice>
  <choice correct="true"><text>Answer option 2 (correct)</text></choice>
  </checkboxgroup>
  </choiceresponse>

   <solution>
   <div class="detailed-solution">
   <p>Solution or Explanation Heading</p>
   <p>Solution or explanation text</p>
   </div>
   </solution>

  </problem>

======
Tags
======

* ``<choiceresponse>`` (required): Specifies that the problem contains options
  for learners to choose from.
* ``<checkboxgroup>`` (required): Specifies that the problem is a checkbox problem.
* ``<choice>`` (required): Designates an answer option.

**Tag:** ``<choiceresponse>``

Specifies that the problem contains options for learners to choose from.

  Attributes

  (none)

  Children

  ``<checkboxgroup>``

**Tag:** ``<checkboxgroup>``

Specifies that the problem is a checkbox problem.

  Attributes

  .. list-table::
     :widths: 20 80

     * - Attribute
       - Description
     * - label (required)
       - Specifies the name of the response field.

  Children

  ``<choice>`` 

**Tag:** ``<choice>``

Designates an answer option.

  Attributes

  .. list-table::
     :widths: 20 80

     * - Attribute
       - Description
     * - true (at least one required)
       - Indicates a correct answer. For checkbox problems, one or more
         ``<choice>`` tags can contain a correct answer.
     * - false (at least one required)
       - Indicates an incorrect answer.

  Children
  
  (none)


.. _Using edX Insights: http://edx.readthedocs.org/projects/edx-insights/en/latest/

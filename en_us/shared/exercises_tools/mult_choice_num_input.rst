.. _Multiple Choice and Numerical Input:

############################################
多项选择和数字输入题
############################################

如果需要，您可以将多选题和数字输入题结合成一个问题。学生不仅在选项中选择答案，还可以提供更多指定信息、

.. image:: ../../../shared/building_and_running_chapters/Images/MultipleChoice_NumericalInput.png
  :alt: Image of a multiple choice and numerical input problem

.. note:: 目前学生只能在文本框中输入数字。不能输入文字或数学表达式。

.. _Create an MCNI Problem:

********************************************************
创建一个多选和数字输入题
********************************************************

如何创建一个多选和数字输入题：

#.在您想创建问题的单元内点击 **添加新组件** 下的 **问题** ，然后点击 **高级** 项。
#. 点击 **空白高级问题** 。
#. 在出现的组件中点击 **编辑** 。
#. 在组件编辑器中，粘贴以下代码。
#. 用您的文本替换示例问题和回答选项。
#. 点击 **保存** 。

.. _MCNI Problem Code:

************************************************
多项选择和数字输入问题代码
************************************************

.. code-block:: xml

  <problem>
  The numerical value of pi, rounded to two decimal points, is 3.24.
  <choicetextresponse>
  <radiotextgroup>
  <choice correct="false">True.</choice>
  <choice correct="true">False. The correct value is <numtolerance_input answer="3.14"/>.</choice>
  </radiotextgroup>
  </choicetextresponse>
  </problem>

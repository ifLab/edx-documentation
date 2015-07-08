.. _Problem Written in LaTeX:

############################
LaTeX问题
############################

.. warning:: 这种问题类型是原生的，而且不被支持。默认情况下，Studio不能创建这类问题。在创建LaTeX问题之前，您必须更改课程高级设置。
  谨慎使用此类问题。

如果您有LaTeX问题，您可以将这个问题类型的代码转换为XML。在您将代码粘贴到LaTeX编辑器以后，您只需要做一些较小的改动。


.. note:: 如果您想使用LaTeX来排版数学表达式。
          在您还没写的问题中，使用`MathJax <http://www.mathjax.org>` 和任何一种其他问题模板。
          更多关于在Studio中使用MathJax创建数学表达式的信息请参考 *A Brief Introduction to MathJax in Studio* 。

.. image:: ../../../shared/building_and_running_chapters/Images/ProblemWrittenInLaTeX.png
 :alt: Image of a problem written in LaTeX

************************************
创建LaTeX问题
************************************

要创建LaTeX问题，您需要：

#. 在您的课程中开启policy key。

   #. 在Studio中点击 **设置** ，点击 **高级设置** 。
   #. 在 **开启LaTeX编译器** 的policy key域，将 **false** 改成 **true** 。
   #. 在页面底部点击 **保存** 。

#. 在您想创建问题的单元中，在 **添加新组件** 下点击 **问题** ，然后点击 **高级** 栏 。
#. 点击 **LaTeX问题** 。
#. 在组件编辑器中点击 **编辑** 。
#. 在编辑器左下角点击 **开启LaTeX源编译器** 。
#. 将示例代码替换为您的代码。您也可以点击右下角的 **上传** 按钮，从计算机内上传Latex文件到编辑器中。
#. 在LaTeX源编译器的左下角，点击 **保存并编译为edX XML** 。

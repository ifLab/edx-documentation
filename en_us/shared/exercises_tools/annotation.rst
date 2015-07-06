.. _Annotation:

###################
注释问题
###################


在注释问题中，导师将文本区域中的指定部分标记为高亮，并就此部分提问。
学生将光标移到高亮文本时，问题出现。问题同时在文本框下方与回答区一起出现。

注释问题要求学生就指定文字进行回答。问题在学生将光标移到高亮文本时出现，
这样学生可以一边阅读一边思考问题。

.. image:: ../../../shared/building_and_running_chapters/Images/AnnotationExample.png
  :alt: Annotation problem

****************************
创建注释问题
****************************

要创建注释问题，您需要在课程中添加注释高级组件，为问题添加 **说明** 和 **导向讨论** 部分，
并添加 **注释问题** 部分。

#. 添加注释高级组件。

    #. 在 **设置** 菜单选择 **高级设置** 。

    #. 在 **高级模块列表** 中将您的光标置于框架之间。

    #. 输入以下值。确保包含引号。

       ``"annotatable"``

    4. 在页面最下方点击 **保存修改** 。

       页面自动更新。在页面顶端，您将看到已保存修改的提示信息。

    5. 回到您想添加特定问题的单元。可用组件列表中现在包含了高级组件。

       .. image:: ../../../shared/building_and_running_chapters/Images/AdvancedComponent.png
          :alt: Image of the Add a New Component panel with the Advanced component option

2. 在问题中添加 **说明** 和 **导向讨论** 部分。

    #. 在您想添加问题的单元中， **添加新组件** 下方点击 **高级** 。
    #. 在问题列表中选择 **注释** 。
    #. 在出现的组件中点击 **编辑** 。
    #. 在组件编辑器中，用您的代码将示例代码替换掉。
    #. 点击 **保存** 。

3. 为问题添加 **注释问题** 部分。

    #. 在注释组件下，创建一个新的空白高级问题组件。

    #. 复制以下代码粘贴在高级问题组件中，用您的信息替换占位符。

        .. code-block:: xml

          <problem>
              <annotationresponse>
                  <annotationinput>
                    <text>PLACEHOLDER: Text of annotation</text>
                      <comment>PLACEHOLDER: Text of question</comment>
                      <comment_prompt>PLACEHOLDER: Type your response below:</comment_prompt>
                      <tag_prompt>PLACEHOLDER: In your response to this question, which tag below
                      do you choose?</tag_prompt>
                    <options>
                      <option choice="incorrect">PLACEHOLDER: Incorrect answer (to make this
                      option a correct or partially correct answer, change choice="incorrect"
                      to choice="correct" or choice="partially-correct")</option>
                      <option choice="correct">PLACEHOLDER: Correct answer (to make this option
                      an incorrect or partially correct answer, change choice="correct" to
                      choice="incorrect" or choice="partially-correct")</option>
                      <option choice="partially-correct">PLACEHOLDER: Partially correct answer
                      (to make this option a correct or partially correct answer,
                      change choice="partially-correct" to choice="correct" or choice="incorrect")
                      </option>
                    </options>
                  </annotationinput>
              </annotationresponse>
              <solution>
                <p>PLACEHOLDER: Detailed explanation of solution</p>
              </solution>
            </problem>

#. 点击 **保存** 。

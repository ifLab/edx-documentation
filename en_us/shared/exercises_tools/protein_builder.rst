.. _Protein Builder:
.. _Protein Builder:

############################
Protex蛋白质构建工具
############################

Protex蛋白质构建工具让学生通过把氨基酸串联起来创建一个特殊的蛋白质形状。如下图所示,目标蛋白质的形状是一个简单的线。



.. image:: ../../../shared/building_and_running_chapters/Images/ProteinBuilder.png
  :alt: Image of the protein builder

.. _Create the Protein Builder:

********************************
创建一个蛋白质构建工具
********************************

要创建一个蛋白质构建工具:

#. 在**添加新组件**下方, 点击**问题*, 然后点击**空白的高级问题**.
#. 在出现的组件中, 点击**编辑**.
#. 在组件编辑器中,复制下面的问题组件代码.
#. 按你所需修改代码,然后点击 **Save**.

.. _Protein Builder Code:

*************************
蛋白质构建问题代码
*************************

.. code-block:: xml

  <problem>
      <p>The protein builder allows you string together the building blocks of proteins, amino acids, and see how that string will form into a structure. You are presented with a goal protein shape, and your task is to try to re-create it. In the example below, the shape that you are asked to form is a simple line.</p> 
     <p>Be sure to click "Fold" to fold your protein before you click "Check".</p>

  <script type="loncapa/python">

  def protex_grader(expect,ans):
    import json
    ans=json.loads(ans)
    if "ERROR" in ans["protex_answer"]:
      raise ValueError("Protex did not understand your answer. Try folding the protein.")
    return ans["protex_answer"]=="CORRECT"

  </script>
 
    <text>
      <customresponse cfn="protex_grader">
        <designprotein2dinput width="855" height="500" target_shape="W;W;W;W;W;W;W"/>
      </customresponse>
    </text>
    <solution>
      <p>
        Many protein sequences, such as the following example, fold to a straight line.You can play around with the protein builder if you're curious.
      </p>
      <ul>
        <li>
            Stick: RRRRRRR
        </li>
      </ul>
    </solution>
  </problem>

在这些代码中:
 
* **width** 和 **height** 指定这个应用的像素大小.
* **target_shape** 列出氨基酸,按指定的顺序结合。创建你叫你学生创建的形状。这个列表只能包含以下的字母每个字母和相应的氨基酸一一对应，(这个列表出现在蛋白质构建器的左上角)。


  .. list-table::
     :widths: 15 15 15 15
     :header-rows: 0

     * - A
       - R
       - N
       - D
     * - C
       - Q
       - E
       - G
     * - H
       - I
       - L
       - K
     * - M
       - F
       - P
       - S
     * - T
       - W
       - Y
       - V

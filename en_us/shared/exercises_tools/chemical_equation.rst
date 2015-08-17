.. _Chemical Equation:

################################
化学方程式问题
################################

化学方程式问题允许学生输入一个输入表示化学方程式的文本到输入框中。系统会把这个文本转化成一个化学方程式在输入框下方。评分器会通过使用你创建并嵌入问题中的Python脚本学生的回答给学生评分。


.. image:: ../../../shared/building_and_running_chapters/Images/ChemicalEquationExample.png
 :alt: Image of a chemical equation response problem

************************************
创建一个化学方程式问题
************************************

化学方程式问题使用MathJax创建公式。更多关于Studio中MathJax的相关信息,请查看:ref:`MathJax in Studio`.

要创建一个化学方程式问题:

#. 在你想要创建化学方程式的单元里面, 在**添加新组件里面**点击**问题**, 然后点击**高级**标.
#. 点击 **空白的高级问题**.
#. 在出现的组件中, 点击**Edit**.
#. 在组件编辑器里, 复制下面的代码.
#. 点击 **保存**.

==========================================
化学方程式问题代码示例
==========================================

.. code-block:: xml

  <problem>
    <startouttext/>
    <p>Some problems may ask for a particular chemical equation. Practice by writing out the following reaction in the box below.</p>
    
  \( \text{H}_2\text{SO}_4 \longrightarrow \text { H}^+ + \text{ HSO}_4^-\)

    <customresponse>
      <chemicalequationinput size="50" label="Enter the chemical equation"/>
      <answer type="loncapa/python">

  if chemcalc.chemical_equations_equal(submission[0], 'H2SO4 -> H^+ + HSO4^-'):
      correct = ['correct']
  else:
      correct = ['incorrect']

      </answer>
    </customresponse>
    <p>Some tips:</p>
    <ul>
    <li>Use real element symbols.</li>
    <li>Create subscripts by using plain text.</li>
    <li>Create superscripts by using a caret (^).</li>
    <li>Create the reaction arrow (\(\longrightarrow\)) by using "->".</li>
    </ul>

    <endouttext/>
  
   <solution>
   <div class="detailed-solution">
   <p>Solution</p>
   <p>To create this equation, enter the following:</p>
     <p>H2SO4 -> H^+ + HSO4^-</p>
   </div>
   </solution>
  </problem>

.. _Chemical Equation Problem XML:

************************************
化学方程式问题XML
************************************

============
模板
============

.. code-block:: xml

  <problem>
    <startouttext/>
    <p>Problem text</p>

    <customresponse>
      <chemicalequationinput size="NUMBER" label="LABEL TEXT"/>
      <answer type="loncapa/python">

  if chemcalc.chemical_equations_equal(submission[0], 'TEXT REPRESENTING CHEMICAL EQUATION'):
      correct = ['correct']
  else:
      correct = ['incorrect']

      </answer>
    </customresponse>

    <endouttext/>
  
   <solution>
   <div class="detailed-solution">
   <p>Solution or Explanation Header</p>
   <p>Solution or explanation text</p>
   </div>
   </solution>
  </problem>

======
标签
======

* ``<customresponse>``: 指定这个问题是一个化学方程式问题. 
* ``<chemicalequationinput>``: 指定这个化学方程式问题的答案. 
* ``<answer type=loncapa/python>``: 包含这个问题中评分器的Python脚本.

**标签:** ``<customresponse>``

I指定这个问题有一个自定义回答. ``<customresponse>`` 标签必须用``<chemicalequation>``标签围绕.

  属性

  (无)

  子标签

  * ``<chemicalequationinput>``
  * ``<answer>``

**标签:** ``<chemicalequationinput>``

指定这个问题的答案使用一个化学方程式并且创建一个回答框供学生输入法答案。


  属性

  .. list-table::
     :widths: 20 80

     * - 属性
       - 描述
     * - 大小 
       - 指定这个回答框内字体的大小.
     * - 标签 (必选)
       - Contains the text of the principal question in the problem.

  子标签
  
  (none)

**标签:** ``<answer>``

包含这个问题的Python脚本评分器.

  属性

  .. list-table::
     :widths: 20 80

     * - 属性
       - 描述
     * - 类型 (必选) 
       - 必须是"loncapa/python".

  子标签
  
  (无)
     

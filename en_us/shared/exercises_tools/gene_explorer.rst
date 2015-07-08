.. _Gene Explorer:

##################
Gene Explorer工具
##################

 `UMB <http://www.umb.edu/>`_ 生物学院的Gene Explorer (GeneX)，
模拟一个小型假定真核生物基因转录、剪接、处理，和翻译的过程。
GeneX允许学生在基因序列中制作特定突变，并计算和显示突变在mRNA和蛋白质上的影响。

Gene Explorer有如下特别作用：

#. 找到启动子和终止子
#. 读DNA序列以产出pre-mRNA
#. 找到剪接位点
#. 剪接mRNA
#. 找到起始密码子
#. 翻译mRNA

.. image:: ../../../shared/building_and_running_chapters/Images/GeneExplorer.png
  :alt: Image of the Gene Explorer

 更多关于Gene Explorer的信息，请参阅 `The Gene Explorer <http://intro.bio.umb.edu/GX/>`_.

********************
Gene Explorer代码
********************

.. code-block:: xml

  <problem>
  <p>Make a single base pair substitution mutation in the gene below that results in a protein that is longer than the protein produced by the original gene. When you are satisfied with your change and its effect, click the <b>SUBMIT</b> button.</p>
  <p>Note that a "single base pair substitution mutation" is when a single base is changed to another base; for example, changing the A at position 80 to a T. Deletions and insertions are not allowed.</p>
  <script type="loncapa/python">
  def genex_grader(expect,ans):
      if ans=="CORRECT": return True
      import json
      ans=json.loads(ans)
      return ans["genex_answer"]=="CORRECT"
  </script>
  <customresponse cfn="genex_grader">
  <editageneinput width="818" height="1000" dna_sequence="TAAGGCTATAACCGAGATTGATGCCTTGTGCGATAAGGTGTGTCCCCCCCCAAAGTGTCGGATGTCGAGTGCGCGTGCAAAAAAAAACAAAGGCGAGGACCTTAAGAAGGTGTGAGGGGGCGCTCGAT" genex_dna_sequence="TAAGGCTATAACCGAGATTGATGCCTTGTGCGATAAGGTGTGTCCCCCCCCAAAGTGTCGGATGTCGAGTGCGCGTGCAAAAAAAAACAAAGGCGAGGACCTTAAGAAGGTGTGAGGGGGCGCTCGAT" genex_problem_number="2"/>
  </customresponse>
  </problem>

在此代码中：

* **width** 和 **height** 制定应用的像素范围。
* **genex_dna_sequence** 是问题打开时的默认DNA序列。
* **dna_sequence** 包含应用程序状态和学生答案。该值必须和 **genex_dna_sequence** 相同。
* **genex_problem_number** 指定问题的编号。 这个编号基于MITx 7.00x 课程中的五个基因编辑器问题。
比如，如果您希望这个问题看起来像7.00x课中的第二个基因编辑器问题，你可以将 **genex_problem_number** 的值设为2。
编号必须是1、2、3、4或5。

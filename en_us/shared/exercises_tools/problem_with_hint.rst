 .. _Problem with Adaptive Hint:

################################
带适应性提示的问题
################################

一个带适应性提示的问题评估学生的回答，然后给学生以反馈或基于回答的提示，以便学生能在下一次尝试时更有可能做出正确回答。这些问题可以是文本输入问题或多选问题。

.. image:: ../../../shared/building_and_running_chapters/Images/ProblemWithAdaptiveHintExample.png
 :alt: Image of a problem with an adaptive hint

******************************************
创建一个带适应性提示的问题
******************************************

创建一个上面的问题：

#. 在你想在其中创建问题的单元中，点击位于 **添加新的组件** 下方的 **问题** ，然后点击 **高级** 标签
#. 点击 **带适应性提示的问题**
#. 在出现的组件中，点击 **编辑**
#. 在组件编辑中，用下列代码替换示例代码
#. 点击 **保存**

.. code-block:: xml

    <problem>
	    <text>
	        <script type="text/python" system_path="python_lib">
	def test_str(expect, ans):
	  print expect, ans
	  ans = ans.strip("'")
	  ans = ans.strip('"')
	  return expect == ans.lower()

	def hint_fn(answer_ids, student_answers, new_cmap, old_cmap):
	  aid = answer_ids[0]
	  ans = str(student_answers[aid]).lower()
	  print 'hint_fn called, ans=', ans
	  hint = ''
	  if '10' in ans:
	     hint = 'If the ball costs 10 cents, and the bat costs one dollar more than the ball, 
	     how much does the bat cost? If that is the cost of the bat, how much do the ball and 
	     bat cost together?'
	  elif '.05' in ans:
	     hint = 'Make sure to enter the number of cents as a whole number.'

	  if hint:
	    hint = "&lt;font color='blue'&gt;Hint: {0}&lt;/font&gt;".format(hint)
	    new_cmap.set_hint_and_mode(aid,hint,'always')
	        </script>
	        <p>If a bat and a ball cost $1.10 together, and the bat costs $1.00 more than the 
	        ball, how much does the ball cost? Enter your answer in cents, and include only 
	        the number (that is, do not include a $ or a ¢ sign).</p>
	        <p>
	            <customresponse cfn="test_str" expect="5">
	                <textline correct_answer="5" label="How much does the ball cost?"/>
	                <hintgroup hintfn="hint_fn"/>
	            </customresponse>
	        </p>
	    </text>
    </problem>

.. _Problem with Adaptive Hint XML:

*********************************
带适应性提示XML的问题
*********************************

========
模板
========

.. code-block:: xml

	<problem>
	  <text>
	    <script type="text/python" system_path="python_lib">
	def test_str(expect, ans):
	  print expect, ans
	  ans = ans.strip("'")
	  ans = ans.strip('"')
	  return expect == ans.lower()

	def hint_fn(answer_ids, student_answers, new_cmap, old_cmap):
	  aid = answer_ids[0]
	  ans = str(student_answers[aid]).lower()
	  print 'hint_fn called, ans=', ans
	  hint = ''
	  if 'incorrect answer 1' in ans:
	     hint = 'hint for incorrect answer 1'
	  elif 'incorrect answer 2' in ans:
	     hint = 'hint for incorrect answer 2'

	  if hint:
	    hint = "&lt;font color='blue'&gt;Hint: {0}&lt;/font&gt;".format(hint)
	    new_cmap.set_hint_and_mode(aid,hint,'always')
	</script>
	    <p>TEXT OF PROBLEM</p>
	    <p>
	      <customresponse cfn="test_str" expect="ANSWER">
	        <textline correct_answer="answer" label="LABEL TEXT"/>
	        <hintgroup hintfn="hint_fn"/>
	      </customresponse>
	    </p>
	  </text>
	</problem>

.. note:: 如果你提供的提示包含字符，字符必需是小写的

========
标签
========

* ``<text>``: 在问题中包围脚本和文本
* ``<customresponse>``: 表示这个问题有一个客户回答
* ``<textline>``: 在LMS中创建一个回答域，学生在其中输入回答
* ``<hintgroup>``: 指定问题至少包含一个提示

**标签：** ``<customresponse>``

  属性

  （空）

  子标签

     * ``<textline>``
     * ``<hintgroup>``

**标签：** ``<textline>``

  属性

  .. list-table::
     :widths: 20 80
     :header-rows: 1

     * - 属性
       - 描述
     * - 标注（必需）
       - 包含问题的文本
     * - 大小（可选）
       - 指定LMS中回答域的大小，以字符为单位
     * - 隐藏（可选）
       - 如果设为 "true"，学生就不能看到回答域
     * - 答案（可选）
       - 问题的答案。提供包含字母的答案，所有字母 **必需为小写**。（学生的回答是大小写不敏感的，他们可以含有大写和小写字母。）

  子标签
  
  （空）

**标签：** ``<hintgroup>``

  属性

  .. list-table::
     :widths: 20 80
     :header-rows: 1

     * - 属性
       - 描述
     * - hintfn
       - 必需设置为 **hint_fn** 也就是，标签必需是这样的 ``<hintgroup hintfn="hint_fn"/>``).
       

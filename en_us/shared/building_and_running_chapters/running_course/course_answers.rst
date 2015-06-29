.. _Review_Answers:

############################
回答问题数据
############################

您可以查阅某个学生对于某个问题提交的答案、下载课程范围内的答题数据报告，或查阅某个问题的答案立方图。

* :ref:`Student_Answer_Submission`

* :ref:`Student_Answer_Distribution`

* :ref:`score_histogram`

Student answer distribution data, including both charts and reports, is also
available from edX Insights. For more information, see `Using edX Insights`_.

.. _Student_Answer_Submission:

************************************************************
查看某个学生的答案及答题历史记录
************************************************************

您可以查看某个学生关于某道题目提交的具体回答内容、回答正确需要尝试的次数，
以及答案提交日期、时间。您可通过用户名锁定学生。

如何查看学生提交的内容：

#. 查看课程现况

#. 单击“课件”，导航至包含该问题的课程单元

#. 查看问题，单击问题下方的“提交历史记录”

#. 输入您想查看学生的用户名，单击页面底部的“查看历史记录”，即出现该生回答问题的信息

随便单击查看窗口外的页面即可关闭窗口。
   
.. _Student_Answer_Distribution:

****************************************
学生答题分布
****************************************

您可下载学生答题分布数据的CSV文件。文件中显示的答题类型包括以下几类：

* 多项选择 (``<choiceresponse>``)
* 下拉列表选择 (``<optionresponse>``)
* 单项选择 (``<multiplechoiceresponse>``)
* 数字输入 (``<numericalresponse>``)
* 文本输入 (``<stringresponse>``)
* 数学表达式输入 (``<formularesponse>``)

该文件中，有一行显示的是您学生选择的所有“问题-答案”配对。
例如，一道问题出现了五种意见不同的答案，则文件中会显示五行，
每一行至少代表一名学生的观点。如果您在Studio中设置了带有“随机选择”功能的问题，
则会另外再开一行。详见 :ref:`Problem Settings`.

CSV文件包含以下几列：

.. list-table::
   :widths: 20 60
   :header-rows: 1

   * - 列
     - 描述
   * - 模块ID
     - 即提问模块的永久ID
   * - 部分ID
     - 如果提问模块包含多个问题，每个问题都有自己的永久ID。
       如果提问模块只包含一个问题，则该值与模块ID相同。
        
   * - 正确回答
     - **答案值** 不正确则为0，正确则为1
       
   * - 回答次数
     - 即学生最近提交某个答案的次数。
       假设本值为X，如果某个问题的 **尝试** 值大于1，
       则每个学生回答该答案的最大次数应在1~X之间，
       哪怕该答案已被尝试多次。
       
   * - 值ID
     - 即单选、多选题中每个选项的永久ID。
       其他提醒则本值为空。
       
   * - 答案值
     - 即多选、下拉列表选择、单选题选项的文本标签，
       以及数字输入、文本输入、表达式输入的值。
       
   * - 多样化
     - 对于设置了“随机选择”的题目，每道题目的变体均有一个“变体”ID。
       没有设置“随机选择”的题目则本值为空。即某道问题的显示名
       
       
   * - 题目显示名
     - 即选项或文本输入字段上方的问题可访问性标签。
   * - 提问
     - 在Studio的“简易编辑器”中，该文本通常用两对角括号表示（>>问题<<）。
       没有设置访问性标签的问题则本值为空。
       
       

输入的值按照分类从左到右排列。

.. _Download_Answer_Distributions:

===================================================
下载学生答题分布报告
===================================================

edX服务器会定期自动更新学生答题数据的CSV文件。
教师面板中可以查看最新版本的CSV文件链接。

如何下载最新的学生答题数据文件：

#. 查看课程现况

#. 单击“导师”→“数据下载”

#. 将滚动条拖至页面底部，单击 ``{course_id}_answer_distribution.csv``
   文件名

==========================================================================
关于学生答题分布报告的常见问题
==========================================================================

Answers to questions about the student answer distribution report follow.   

**我的课程没有学生答题分布报告，要怎么生成？**

学生答题分布报告是自动生成的，每隔几天会自动更新。 ``{course_id}_answer_distribution.csv`` 
文件位于所有 ``{course_id}_grade_report_{date}.csv`` 文件后面。请一定将滚动条拖到最底部。

**为什么报告里漏掉了几道题目？漏掉的题目属于** :ref:`Review_Answers` **一节中列出来的题目类型。**

本报告中的问题为2013年十月份至2014年三月份之前的问题，且至少要有一名学生回答。

**为什么有些问题看不见“答案值”？**

对于单选、多选题而言，只有2014年三月初之后选择的选项才有“答案值”。
2013年十月至2014年3月初之间选择的选项也在报告中，但没有“答案值”。
“值ID”显示的是这些选项的永久ID，比如“choice_1”、“choice_2”。

**为什么我看不见有些题目的“Question”值？**

“Question”列中的值为该题的可访问性标签。更多关于设置问题标签的信息可以参考 :ref:`Create
Exercises`.

并且，对于设置了“随机选择”的题目，如果2014年三月初之前都没有人给出一个明确的答案，则该答案的“Question”值为空。

**我的学生说他们回答了一个问题，报告中确没有显示，这是怎么回事？**

本报告只包含“最大尝试次数”超过1次的问题。

**题目发布后不久，我对题目做了更改。我怎样才能判断更改之前有哪些学生回答了我的问题？**

某道问题的“计数”值反映的是这道问题的历史操作记录。
如果问题发布后您做出了更改，则无论更改前后，您的要求均不能满足。

**我在电子制表软件中查看报告时，为什么相同的答案显示在不同的两列中？**

有些制表软件为了显示方便，会自动转换CSV报告中的数据。
比如，有些学生回答“0.5”，有些学生回答“ .5”，
Excel表格会将这两个答案的“答案值”都显示为“0.5”。
如果您再发现您所说的情况，可以在文本编辑器中查看原始的CSV文件。

**为什么我在制表软件中查看报告时，会出现奇怪的字符？**

CSV文件使用的是UTF-8编码，但是有些制表软件无法准确识别UTF-8编码。
比如说，某学生的法语答题报告在Microsoft Excel for Mac软件和OpenOffice Calc软件中显示的结果就不同。

  Answer Values in Microsoft Excel for Mac:

   .. image:: ../../../shared/building_and_running_chapters/Images/student_answer_excel.png
     :alt: A spreadsheet that replaces accented French characters with underscores

  Answer Values in OpenOffice Calc:

   .. image:: ../../../shared/building_and_running_chapters/Images/student_answer_calc.png
     :alt: A spreadsheet that displays accented French characters correctly

如果您再次发现类似问题，可以试着换一种制表软件，比如LibreOffice或者Apache OpenOffice。

==========================================================================
Interpret the Student Answer Distribution Report
==========================================================================

You can use the Student Answer Distribution report to review student responses
to assignments, which can then help you evaluate the structure and completeness
of your courseware and problem components.

As an example, you define a text input question in Studio to have a single
correct answer, "Warfarin". When you produce the Student Answer Distribution
report, you verify that this answer was in fact marked correct: there is a 1 in
the **Correct Answer** column for this **AnswerValue**.

.. image:: ../../../shared/building_and_running_chapters/Images/SAD_Answer_Review.png
    :alt: In Excel, 5 rows show 5 answer values, 4 of which show comprehension of the question, but only 1 answer is marked as correct

However, as you view the report you notice other student answers that you did
not set up to be marked as correct in Studio, but that you might (or might not)
also consider to be correct, such as "Warfarin or Coumadin". The **Correct
Answer** column shows that the other answers were marked incorrect (0), but for
future iterations of your course you may want to revise the question or update
the problem to evaluate additional variations of the answer as correct.

Many spreadsheet applications offer data visualization options, such as charts
or graphs. Charts can help make your students' common misconceptions  easier to
identify.

.. image:: ../../../shared/building_and_running_chapters/Images/SAD_Column_Chart.png
    :alt: In Excel, AnswerValue and Count columns next to each other, values for 4 rows selected, and a column chart of the count for the 4 answers

In this example, the Student Answer Distribution report is open in Microsoft
Excel. To create a chart that shows how many of your students chose various
answers to a multiple choice question, you move the **AnswerValue** and
**Count** columns next to each other. After you click and drag to select the
report cells that contain the data you want to chart, you click the Charts
toolbar and then click the type of chart you want.

.. note:: Refer to the help for the spreadsheet application that you use for information on using these options. You may have to make changes to your spreadsheet, such as reordering columns. Save a copy of the file you originally downloaded as a backup before you begin. 

You can adjust your course content based on common student mistakes. While most
students in this example selected the correct answer, the number of incorrect
answer(s) can guide future changes to the courseware.

.. _score_histogram:

**************************************************
View a Histogram of Scores for a Single Problem
**************************************************

You can view a chart of the score distribution for a specified problem. 

.. note:: To view the score distribution for a problem, you need its unique identifier. You can display a histogram for problems that have the  ``/problem/`` prefix in the unique identifier. See :ref:`find_URL`.

To display the distribution of scores for a problem:

#. View the live version of your course.

#. Click **Instructor**, then click **Analytics**. 

#. In the Score Distribution section, select a problem by using its unique
   identifier.

   The **Analytics** page updates to display a histogram of scores for that
   problem.

   .. image:: ../../../shared/building_and_running_chapters/Images/score_histogram.png
     :alt: Graph of the number of students who received different scores for a
         selected problem

..  **Question**: (sent to Olga 31 Jan 14) this is a tough UI to use: how do they correlate the codes in this drop-down with actual constructed problems? the copy-and-paste UI on the Student Admin page actually works a little better imo. LMS-2522

===================================================
Interpret a Score Histogram
===================================================

The histogram of scores for a selected problem provides the following
information.

   .. image:: ../../../shared/building_and_running_chapters/Images/score_histogram_callouts.png
     :alt: Histogram with indicators for the number of students scored value and
         the x-axis numbers that indicate plotted scores

* The x-axis indicates the number of points that students can receive for the
  problem, unweighted. Although decimal values are marked on the x-axis, each
  score is a whole number. The whole number value at the left of a plotted bar
  is the score that applies to it.

* The y-axis indicates the number of students who have answered and checked the
  problem.

* Above the graph, a number of **students scored** displays. This number
  indicates the total number of database records that exist for the problem: it
  includes not only students who have answered and checked the problem to
  receive a score, but also students who have opened the problem but not yet
  completed it.

* An automated process runs approximately weekly on the edX servers to update
  score histograms. This process runs less frequently than the process that
  updates the student answer distribution report: at certain times during a
  course the number of students shown in a score histogram can be quite
  different than the **Count** for the same problem in a student answer
  distribution report.


.. _Using edX Insights: http://edx-insights.readthedocs.org/en/latest/

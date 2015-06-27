.. _Working with Problem Components:

################################
创建问题组件
################################

******************************
问题组件概况
******************************

问题组件允许您在您课程内容中添加互动式及自动评分的练习。
您可以在Studio下创建不同类型的问题。

通过默认设置，所有问题都会得分，但是不会计算学生的总分。
若您想让这些问题计算学生的总分，修改保存问题的小节的作业类型。

本章讲述的是问题组件的基础知识，即：您与学生所见的视图，每个问题组件的选项。欲知单个问题类型，请见 :ref:`Create Exercises`.

欲知更多信息，请浏览以下主题：

* :ref:`Problem Student View`
* :ref:`Problem Studio View`
* :ref:`Problem Settings`
* :ref:`Modifying a Released Problem`
* :ref:`Additional Work with Problems`
* :ref:`Multiple Problems in One Component`
* :ref:`Problem Randomization`

.. _Problem Student View:

************************************
学生视图下的问题
************************************

凡是出现在edX平台的所有问题均包含以下功能。

.. image:: ../../../shared/building_and_running_chapters/Images/AnatomyOfExercise1.png
 :alt: Image of a problem from a student's point of view, with callouts for 
       elements of the problem

#. **问题文本** 问题文本允许使用任何标准HTML格式。

#. **学生答案填写区域** 学生在此区域输入答案。回答区域的样式随着问题类型而变化。

#. **提交答案** 对于一些问题类型，Studio使用MathJax提交完美的数学公式。

#. **检查按钮** T学生点击检查，查询上交的答案是否争取。若答案正确的话，则出现绿色的打勾符号。

#. **保存按钮** 学生点击保存，保存的是正确的答案，而非提交。因此，学生可回头修改问题的答案。

#. **显示答案按钮** 此按钮是可选择的。学生点击显示答案时，学生能看到正确答案（见上方第2点）和解题说明(见下方第10点）。教师可设置是否开放此功能。

#. **提交答案次数** 教师可设定提交次数限定或不设定提交次数。
   默认情况下，整个课程中所有问题的 **最多尝试次数** 是空值，这表示提交答案次数是无限的。
   如果课程的 **最多尝试次数** 设定为一个特定的值，课程中的每个问题的尝试次数均为这个值，不能设为无限。

   .. image:: ../../../shared/building_and_running_chapters/Images//AnatomyOfExercise2.png
    :alt: Image of a problem from a student's point of view, with callouts for 
          attempts and showing the answer

#. **反馈** 学生点击检查按钮后，所有问题都会显示绿色复选标记或红X。

   .. image:: ../../../shared/building_and_running_chapters/Images//AnatomyofaProblem_Feedback.png
    :alt: Image of feedback checkmark and x from a student's point of view

#. **正确答案** 大多数问题都需要教师指定一个唯一的正确答案。

#. **解析** 教师可以添加一些解析。当学生点击 **显示答案** 按钮时，会显示相关解析。

#. **重置按钮** 此按钮可以清除学生输入的内容，使问题保持原样。
   
   not yet been submitted, and try again to answer the question. If the student
   has already submitted an answer, clicking **Reset** clears the submission
   and, if the problem contains randomized variables and randomization is set
   to **On Reset**, changes the values the student sees in the problem. If the
   number of Maximum Attempts that was set for this problem has been reached,
   the **Reset** button is not visible.

#. **隐藏答案按钮**

   .. image:: ../../../shared/building_and_running_chapters/Images//AnatomyOfExercise3.png
    :alt: A graded assignment shown in the left pane of the LMS for a course

#. **分级** 教师可以决定一组问题是否进行分级。如果一组问题要进行分级的话，课程作业栏就会出现一个钟表图标。

   .. image:: ../../../shared/building_and_running_chapters/Images//clock_icon.png

#. **到期日** 问题是有期限的。过期的问题就不会有检查按钮了，也不能在进行回答或提供回馈了。

.. note:: 问题可以打开或者关闭。关闭的问题没有检查按钮。
          学生仍然可以看见问题，答案和解析，但是不能查看他们自己做的答案，不能提交答案，也不能更改早期的分数。


还有一些题没有立即可见的属性，您可以在Studio中设置这些属性。

*  **随机化** 对于有些问题，教师可以决定是否采用随机生成的方式，这样每个学生的问题都会不同。


*  **问题权重** 在一组特定的问题中，不同问题权重也不同。

*  **标签** 为提高有困难的同学的可访问性，每一个问题都需要有一个描述性标签。
   这个标签通常包含部分或全部的问题文本。大部分的模板会留出标签的位置。您可以在每个题型或者工具类型的文件中找到示例标签。
   

.. _Problem Studio View:

************************************
Studio中的问题视图
************************************

所有的问题都以XML写成。但是，Studio有两个编辑问题的界面：简易编辑器和进阶编辑器。

*  简易编辑器可以让您进行可视化编辑，不必使用XML。

*  进阶编辑器将问题转换为edX的XML标准,您可以直接编辑XML。

通过点击简易编辑器界面右上角的进阶编辑器按钮，您可以随时从简易编辑器切换到进阶编辑器。
但是您不能从进阶编辑器切换到简易编辑器。

.. _Simple Editor:

=================
简易编辑器
=================


When you select the following problem types, the Simple Editor opens with a preformatted example problem.

*  :ref:`Checkbox`: In checkbox problems, students select one or more options
   from a list of possible answers.

*  :ref:`Dropdown`: In dropdown problems, students select one answer from a
   dropdown list.

*  :ref:`Multiple Choice`: Multiple choice problems require students to
   select one answer from a list of choices that appear directly below
   the question.

*  :ref:`Numerical Input`: Numerical input problems require answers that
   include only integers, fractions, and a few common constants and
   operators.

*  :ref:`Text Input`: In text input problems, students enter a short text
   answer to a question.

下图显示的是简易编辑器中的多项选择题。

.. image:: ../../../shared/building_and_running_chapters/Images//MultipleChoice_SimpleEditor.png
 :alt: The simple editor with numbered callouts for options and an example
     multiple choice problem to demonstrate the formatting.

简单编辑器含有一个工具栏，可将您的问题文本格式化。当您选中文本，点击格式化按钮之后，简单编辑器就可自动将您的文本格式化。

工具栏按钮如下：

1. 创建1级标题
2. 创建多个选项。
3. 创建复选框选项。
4. 创建文本输入选项。
5. 创建数值输入选项。
6. 创建下拉选项。
7. 创建解析，当学生点击显示答案时，就会显示相关解析。
8. 在进阶编辑器中打开问题。
9. 打开格式提示清单。
10. **Accessible Label**: Identify the question as the problem's accessible
    label. No toolbar option is available, but when you surround text with two
    pairs of angle brackets pointing inward (``>>question<<``), screen readers
    use that text as the accessible label for the problem.

    In addition, edX Insights uses the accessible label to identify the
    question in each problem. For more information, see `Using edX Insights`_.

.. _Advanced Editor:

===================
进阶编辑器
===================

 **进阶编辑器** 要用XML打开问题。问题模板包括拖拽，下拉和数学表达式，这些都可在进阶编辑器中直接打开。

下图显示的是进阶编辑器中打开的多项选择题。

.. image:: ../../../shared/building_and_running_chapters/Images//MultipleChoice_AdvancedEditor.png
 :alt: Image of a problem in the advanced editor

以下问题模板可在进阶编辑器中打开。

* :ref:`Circuit Schematic Builder` 在电路原理问题中,学生可以在一个交互式网格中创建和修改电路，并提交计算机生成的电路分析来进行分级

* :ref:`Custom JavaScript` 自定义JavaScript显示和分级问题,您可以通过IFrame将之前用HTML制作的题型并入到Studio中。

* :ref:`Drag and Drop` 拖放问题要求学生能够拖动文本或者将文本放到一张图像的指定位置。

* :ref:`Image Mapped Input` 图像映射输入问题要求学生能够点击一张图像上的指定位置。

* :ref:`Math Expression Input` 数学表达式输入问题还要求学生能够输入数学表达式的文本，如e=m*c^2。

* :ref:`Problem with Adaptive Hint` 这些问题会根据学生的答案给予学生一些回馈或提示。

* :ref:`Problem Written in LaTeX` 这类题型能够将您用LaTeX写好的问题转换为edX格式。注意这种题型仍然在试用中，未来可能不再支持这种题型。

* :ref:`Write Your Own Grader` 自定义Python-评估输入（也被称作“自编分级”题型)能够通过您自己创建的嵌入式Python脚本来评估学生的答案。

.. _Problem Settings:

******************
问题设置
******************

除了问题的文本,您使用问题组件创建的问题包括以下设置。这些设置在组件编辑器中的设置选项卡中。

*  `Display Name`_
*  `Maximum Attempts`_
*  `Problem Weight`_
*  `Randomization`_
*  `Show Answer`_
*  `Show Reset Button`_
*  `Timer Between Attempts`_

.. image:: ../../../shared/building_and_running_chapters/Images/ProbComponent_Attributes.png
 :alt: Image of the Settings tab in a Problem component

===============
显示名称
===============

此设置显示您问题的名称。问题名称将以问题标题的形式显示在LMS和页面上方的条状区域。

.. image:: ../../../shared/building_and_running_chapters/Images/ProbComponent_LMS_DisplayName.png
 :alt: Image of the problem in a unit page from a student's point of view

In addition, edX Insights uses the display name to identify each problem.
Unique, descriptive display names help you identify problems quickly and
accurately for analysis. For more information, see `Using edX Insights`_.

==============================
最多答题次数
==============================

此设置规定学生最多可尝试回答问题次数。系统默认学生的回答次数不受限制。
This setting specifies the number of times a student is allowed to attempt
answering the problem. By default, the course-wide **Maximum Attempts**
advanced setting is null, meaning that the maximum number of attempts for
problems is unlimited. If the course-wide **Maximum Attempts** setting is
changed to a specific number, the **Maximum Attempts** setting for individual
problems defaults to that number, and cannot be set to unlimited.

.. note:: 将问题最多回答次数设置为1或者更多，问题才能出现在学生答题统计报告中，您可以在上课时下载该报告。


.. _Problem Weight:

==============================
问题权重
==============================

.. note:: Studio可以保存所有问题的分数，但是只有这些分数属于某个小节，
          并且这个小节被设定成计分后，才会对学生的期末成绩造成影响。

这项设定可以规定问题的最大分值。问题的分值标在在问题题目后面。

.. image:: ../../../shared/building_and_running_chapters/Images/ProblemWeight_DD.png
 :alt: Image of a problem from a student's point of view, with the possible 
       points circled

系统默认，问题组件中的每一个应字段或者“答题框”都值1分。
每一个问题组件都包含多个应字段。
例如，上述问题组件包含一个下拉问题，这个下拉问题包含三个独立问题需要学生来回答，因此它有三个应字段。

下面的问题组件包含一道文本输入题，就只有一个应字段。

.. image:: ../../../shared/building_and_running_chapters/Images/ProblemWeight_TI.png
 :alt: Image of a text input problem from a student's point of view

计算分数
****************

学生回答问题得分由以下公式计算得出：

**分数=问题权重×（正确答案/输入总和）**

*  **分数** 指的是学生回答问题所得的分数。

*  **问题权重** 指的是回答这个问题所能获得的最高分数。

*  **正确答案** 指的是所有回答中正确答案的数量。

*  **输入总和** 指的是所有这个题组本身所拥有的问题数量总和。

**范例**

接下来是一些计算分数的例子。

*Example 1*

A problem's **Weight** setting is left blank. The problem has two
response fields. Because the problem has two response fields, the
maximum score is 2.0 points.

If one response field contains a correct answer and the other response
field contains an incorrect answer, the student's score is 1.0 out of 2
points.

*Example 2*

A problem's weight is set to 12. The problem has three response fields.

If a student's response includes two correct answers and one incorrect
answer, the student's score is 8.0 out of 12 points.

*Example 3*

A problem's weight is set to 2. The problem has four response fields.

If a student's response contains one correct answer and three incorrect
answers, the student's score is 0.5 out of 2 points.

.. _Randomization:

===============
Randomization
===============

This setting specifies whether certain values in your problem change each time
a different student accesses the problem, or each time a single student tries
to answer the problem. For example, the highlighted values in the problem below
change each time a student submits an answer to the problem.

.. image:: ../../../shared/building_and_running_chapters/Images/Rerandomize.png
 :alt: The same problem shown twice, with color highlighting on values that 
       can change

If you want to change, or "randomize," specific values in your problem, you
have to do both the following:

* Make sure that your problem contains a Python script that randomizes the
  values that you want.

* Enable randomization in the Problem component. 

.. note:: Note that specifying this **Randomization** setting is different 
 from *problem randomization*. The **Randomization** setting randomizes
 variables within a single problem. Problem randomization offers different
 problems or problem versions to different students. For more information, see
 :ref:`Problem Randomization`.

To enable randomization, select an option for the **Randomization** setting.
This setting has the following options.

+-------------------+--------------------------------------+
| **Always**        | Students see a different version of  |
|                   | the problem each time they click     |
|                   | **Check**.                           |
+-------------------+--------------------------------------+
| **On Reset**      | Students see a different version of  |
|                   | the problem each time they click     |
|                   | **Reset**.                           |
+-------------------+--------------------------------------+
| **Never**         | All students see the same version    |
|                   | of the problem. This is the default. |
+-------------------+--------------------------------------+
| **Per Student**   | Individual students see the same     |
|                   | version of the problem each time     |
|                   | they look at it, but that version    |
|                   | is different from the version that   |
|                   | other students see.                  |
+-------------------+--------------------------------------+

.. note:: The edX Platform has a 20-seed limit for randomization.

.. _Show Answer:

===============
Show Answer
===============

This setting defines when the problem shows the answer to the student.
This setting has the following options.

+-------------------+--------------------------------------+
| **Always**        | Always show the answer when the      |
|                   | student clicks the **Show Answer**   |
|                   | button.                              |
+-------------------+--------------------------------------+
| **Answered**      | Show the answer after the student    |
|                   | tries to answer the problem.         |
|                   |                                      |
|                   | If the question can be, and is,      |
|                   | reset, the answer                    |
|                   | is not shown until the student tries |
|                   | the problem again. (When a student   |
|                   | answers a question, the question is  |
|                   | considered to be                     |
|                   | both attempted and answered. When    |
|                   | the question is reset, the question  |
|                   | is still attempted, but not yet      |
|                   | answered.)                           |
+-------------------+--------------------------------------+
| **Attempted**     | Show the answer after the student    |
|                   | tries to answer the problem.         |
|                   |                                      |
|                   | If the question can be, and is,      |
|                   | reset, the answer                    |
|                   | *continues to show*.                 |
|                   | (When a student answers a question,  |
|                   | the question is considered to be     |
|                   | both attempted and                   |
|                   | answered. When the question is       |
|                   | reset, the question is still         |
|                   | attempted, but not yet answered.)    |
+-------------------+--------------------------------------+
| **Closed**        | Show the answer after the student    |
|                   | has used up all his attempts to      |
|                   | answer the problem or the due date   |
|                   | has passed.                          |
+-------------------+--------------------------------------+
| **Finished**      | Show the answer after the student    |
|                   | has answered the problem correctly,  |
|                   | the student has no attempts left, or |
|                   | the problem due date has passed.     |
+-------------------+--------------------------------------+
| **Correct or      | Show the answer after the student    |
| Past Due**        | has answered the problem correctly   |
|                   | or the problem due date has passed.  |
+-------------------+--------------------------------------+
| **Past Due**      | Show the answer after the due date   |
|                   | for the problem has passed.          |
+-------------------+--------------------------------------+
| **Never**         | Never show the answer. In this case, |
|                   | the **Show Answer** button does not  |
|                   | appear next to the problem in Studio |
|                   | or in the LMS.                       |
+-------------------+--------------------------------------+

.. _Show Reset Button:

=================
Show Reset Button
=================

This setting defines whether a **Reset** button is visible on the problem.
Students can click **Reset** to clear any input that has not yet been submitted,
and try again to answer the problem. If the student has already submitted an
answer, clicking **Reset** clears the submission and, if the problem contains
randomized variables and randomization is set to **On Reset**, changes the
values the student sees in the problem. If the number of Maximum  Attempts that
was set for this problem has been reached, the **Reset** button is not visible.

This problem-level setting overrides the course-level **Show Reset Button for
Problems** setting.

.. _Timer Between Attempts:

=======================
Timer Between Attempts
=======================

This setting specifies the number of seconds a student must wait between
submissions for a problem that allows multiple attempts. If the value is 0, the
student can attempt the problem again immediately after an incorrect attempt.

Adding required wait time between attempts can help to prevent learners from
simply guessing when multiple attempts are allowed.

If a learner attempts a problem again before the required time has elapsed, she
sees a message below the problem indicating the remaining wait time.

.. image:: ../../../shared/building_and_running_chapters/Images/problem_attempt_timer.png
 :alt: Problem with message that learner must wait before attempting again


.. _Modifying a Released Problem:

*********************************
Modifying a Released Problem
*********************************

.. warning:: Be careful when you modify problems after they have been 
 released! Changes that you make to published problems can affect the student
 experience in the course and analysis of course data.

After a student submits a response to a problem, the edX Learning Management
System (LMS) stores the student's response, the score that the student
received, and the maximum score for the problem. For problems with a **Maximum
Attempts** setting greater than 1, the LMS updates these values each time the
student submits a new response to a problem. However, if an instructor changes
a problem or its attributes, existing student information for that problem is
not automatically updated.

For example, you may release a problem and specify that its answer is 3.
After some students have submitted responses, you notice that the answer
should be 2 instead of 3. When you update the problem with the correct
answer, the LMS does not update scores for students who originally answered 
2 for the problem and received the wrong score.

For another example, you may change the number of response fields to
three. Students who submitted answers before the change have a score of
0, 1, or 2 out of 2.0 for that problem. Students who submitted answers
after the change have scores of 0, 1, 2, or 3 out of 3.0 for the same
problem.

If you change the weight setting for the problem in Studio, however, existing
student scores update when the student's **Progress** page is refreshed. In a
live section, students will see the effect of these changes.

===============
Workarounds
===============

If you have to modify a released problem in a way that affects grading, you
have two options within Studio to assure that every student has the opportunity
to submit a new response and be regraded. Note that both options require you to
ask your students to go back and resubmit answers to a problem.

*  In the Problem component that you changed, increase the number of attempts
   for the problem. Then ask all your students to redo the problem.

*  Delete the entire Problem component in Studio and create a new Problem
   component with the content and settings that you want. (If the revisions you
   must make are minor, duplicate the Problem component before you delete it
   and revise the copy.) Then ask all your students to complete the new
   problem.

For information about how to review and adjust student grades in the LMS, see
:ref:`Grades`.

.. _Additional Work with Problems:

************************************
Additional Work with Problems
************************************

You have some further options when you work with problems. You can include more
than one problem in a single problem component, or you can set up a problem
that presents different versions to different students.

.. _Multiple Problems in One Component:

====================================
Multiple Problems in One Component
====================================

You may want to create a problem that has more than one response type. For
example, you may want to create a numerical input problem, and then include a
multiple choice question about the numerical input problem. Or, you may want a
student to be able to check the answers to many problems at one time. To do
this, you can include multiple problems inside a single Problem component. The
problems can be different types.

.. note:: 
  You cannot use a :ref:`Custom JavaScript` in a component that contains more
  than one problem. Each custom JavaScript problem must be in its own
  component.

To create multiple problems in one component, create a new Blank Advanced
Problem component, and then add the XML for each problem in the component
editor. You only need to include the XML for the problem and its answers. You
do not have to include the code for other elements, such as the **Check**
button.

Elements such as the **Check**, **Show Answer**, and **Reset** buttons, as well
as the settings that you select for the Problem component, apply to all of the
problems in that component. Thus, if you set the maximum number of attempts to
3, the student has three attempts to answer the entire set of problems in the
component as a whole rather than three attempts to answer each problem
individually. If a student clicks **Check**, the LMS scores all of the problems
in the component at once. If a student clicks **Show Answer**, the answers for
all the problems in the component appear.

.. _Problem Randomization:

===========================
Problem Randomization
===========================

You may want to present different students with different problems, or
different versions of the same problem. To do this, you'll create a Problem
component for each problem or version in Studio, and then edit your course
outside of Studio to randomize the problem that students see.

Note that *problem randomization* is different from the **Randomization**
setting in Studio. The **Randomization** setting randomizes variables within a
single problem. Problem randomization offers different problems or problem
versions to different students.

.. note:: Creating problems with versions that can be randomized requires you 
 to export your course, edit some of your course's XML files in a text editor,
 and then re-import your course. We recommend that you create a backup copy of
 your course before you do this. We also recommend that you only edit your
 course files in the text editor if you're very familiar with editing XML.

Terminology
************

Sections, subsections, units, and components have different names in the
**Course Outline** view and in the list of files that you'll see after you
export your course and open the .xml files for editing. The following table
lists the names of these elements in the **Course Outline** view and in a list
of files.

.. list-table::
   :widths: 15 15
   :header-rows: 0

   * - Course Outline View
     - File List
   * - Section
     - Chapter
   * - Subsection
     - Sequential
   * - Unit
     - Vertical
   * - Component
     - Discussion, HTML, problem, or video

For example, when you want to find a specific section in your course, you'll
look in the **Chapter** folder when you open the list of files that your course
contains. To find a unit, you'll look in the **Vertical** folder.

.. _Create Randomized Problems:

Create Randomized Problems
****************************

#. In the unit where you want to create a randomized problem, create a separate
   Problem component for each version or problem that you want to randomize.
   For example, if you want to offer four versions or problems, you'll create
   four separate Problem components. Make a note of the 32-digit unit ID that
   appears in the **Unit Identifier** field under **Unit Location**.

#. Export your course. For information about how to do this, see
   :ref:`Exporting and Importing a Course`. Save and extract the .tar.gz file
   that contains your course in a memorable location so that you can find
   it easily.

#. In the list of folders and files, open the **Vertical** folder.

   .. note:: If your unit is not published, open the **Drafts** folder, and 
    then open the **Vertical** folder in the **Drafts** folder.

#. In the **Vertical** folder, locate the .xml file that has the same name as
   the unit ID that you noted in step 1, and then open the file in a text
   editor such as Sublime 2. For example, if the unit ID is
   e461de7fe2b84ebeabe1a97683360d31, you open the
   e461de7fe2b84ebeabe1a97683360d31.xml file.

   The file contains a list of all the components in the unit, together with
   the URL names of the components. For example, the following file contains
   four Problem components.

   .. code-block:: xml
     
       <vertical display_name="Test Unit">
          <problem url_name="d9d0ceb3ffc74eacb29501183e26ad6e"/>
          <problem url_name="ea66d875f4bf4a9898d8e6d2cc9f3d6f"/>
          <problem url_name="2616cd6324704f85bc315ec46521485d"/>
          <problem url_name="88987707294d4ff0ba3b86921438d0c0"/>
       </vertical>

#. Add ``<randomize> </randomize>`` tags around the components for the problems
   that you want to randomize.

   .. code-block:: xml
      
       <vertical display_name="Test Unit">
         <randomize>
            <problem url_name="d9d0ceb3ffc74eacb29501183e26ad6e"/>
            <problem url_name="ea66d875f4bf4a9898d8e6d2cc9f3d6f"/>
            <problem url_name="2616cd6324704f85bc315ec46521485d"/>
            <problem url_name="88987707294d4ff0ba3b86921438d0c0"/>
         </randomize>
       </vertical>

#. After you add the ``<randomize> </randomize>`` tags, save and close the .xml
   file.

#. Re-package your course as a .tar.gz file.

   For information about how to do this on a Mac, see `How to Create a Tar GZip
   File from the Command Line <http://osxdaily.com/2012/04/05/create-tar-gzip/>`_.

   For information about how to do this on a Windows computer, see `How to Make
   a .tar.gz on Windows <http://stackoverflow.com/questions/12774707/how-to-make-a-tar-gz-on-windows>`_.

#. In Studio, re-import your course.

.. note::

  * Once you've implemented randomization, you can only see one of the versions
    or problems in Studio. You can edit that single problem directly in Studio,
    but to edit any of the other problems, you'll have to export your course,
    edit the problems in a text editor, and then re-import the course. This is
    true for instructors as well as course teams.
  
  * A .csv file for student responses contains the responses to each of the
    problems in the problem bank.

.. include:: ../../../shared/exercises_tools/adding_tooltip.rst

.. _Using edX Insights: http://edx.readthedocs.org/projects/edx-insights/en/latest/

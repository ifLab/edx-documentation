.. _Set Course Prerequisites:

#########################
设定入学要求
#########################

也许您想要确保学生在上课前有指定的技能和知识基础。

.. contents:: 内容包括：
 :local:
 :depth: 1


.. _Specify Prerequisite Courses:

****************************
指定先修课程
****************************

您可以要求学生在注册您的课程之前先通过特定的edX课程。
学生将在课程信息页面看到关于课程的入学要求。

.. image:: ../../../shared/building_and_running_chapters/Images/PrereqAboutPage.png
  :width: 500
  :alt: A course About page with prerequisite course information circled

如果学生没有完成先修课程，他们就不能注册您的课程，也不能在学生面板中看到您的课程。
但是与其他课程不同，学生面板不提供此课程课件链接。
学生面板包括先修课程信息页面的链接。学生可以在信息页面注册先修课程。

.. image:: ../../../shared/building_and_running_chapters/Images/Prereq_StudentDashboard.png
  :width: 500
  :alt: The Student Dashboard with an available course and a course that is
      unavailable because it has a prerequisite

要指定先修课程，您必须是当前课程以及先修课程的作者。

#. 在Studio中打开您的课程。
#. 在 **设置** 菜单中选择 **日程表和细节** 。 
#. 在 **日程表和细节** 页面，选择 **要求** 一栏 。 
#. 在 **先修课程** 的下拉列表中选择一门课程。 
#. 在页面底部选择 **保存修改** 。

.. note:: 目前您只能选定一门先修课程。


.. _Require an Entrance Exam:

****************************
设置入学考试
****************************

您可以要求学生在访问您的课程材料之前通过入学考试。
如果课程含有入学考试，注册该课程的学生只能看到 **课程更新与新闻** 页面和 **入学考试** 标签，
直到他们通过入学考试。

.. image:: ../../../shared/building_and_running_chapters/Images/EntEx_LandingPage.png
  :width: 500
  :alt: The Course Updates & News page with the Entrance Exam tab circled on the
      left


学生通过入学考试以后，他们可以访问所有已发布的课程资料。

安装以下步骤设置入学考试。

#. 在Studio中打开您的课程。, open your course.
#. 在 **设置** 菜单中选择 **日程表与细节** 。 On the **Settings** menu, select **Schedule & Details**.
#. 在 **日程表与细节** 页面下滚到 **要求** 部分。 On the **Schedule & Details** page, scroll to the **Requirements** section.
#. 选择 **要求学生访问课程资料之前通过入学考试** 。 Select the **Require students to pass an exam before accessing course
   materials** check box.
#. 在页面底端选择 **保存修改** 。At the bottom of the page, select **Save Changes**.

After you save your changes, Studio automatically creates an **Entrance Exam**
section in your course outline. To add content to your entrance exam, go to the
course outline.

==================================
Best Practices for Entrance Exams
==================================

We strongly recommend that you follow several guidelines to help you and your
students have a positive experience with entrance exams.

* Make sure that your beta testers include the entrance exam when they test
  your other course content.

* Make sure that you mention the entrance exam in the course description on
  your course About page. Otherwise, students will not know about the entrance
  exam before they enroll in your course and try to access course content.

* Add an anouncement at the top of the **Course Updates & News** page that
  contains information and instructions for students who need to take the exam.
  When students first try to access content in a course that has an entrance
  exam, they see the **Course Updates & News** page. We suggest that you
  include the following information.

  * To begin the course entrance exam, students click the **Entrance Exam** tab
    on the left side of the screen.

  * After students complete the entrance exam, they have to click the
    **Entrance Exam** tab again or refresh the page in their browser. When the
    page refreshes, students can see all currently available course content.

    .. image:: ../../../shared/building_and_running_chapters/Images/EntEx_CourseAccordionAfterPass.png
      :width: 500
      :alt: The student view after the student has passed the entrance exam,
          with all available course sections listed in the course accordion

================================================
Create an Entrance Exam from the Course Outline
================================================

You create your course entrance exam from the course outline in Studio.
Creating entrance exam content is just like creating other course content. For
more information, see :ref:`Creating Course Content Index`.

==================================
Adjust Scores in the Entrance Exam
==================================

If you find an error in the exam after students have taken it, and corrections
to the exam are unavoidable, you have several options to rescore the exam for
individual students. These options are available on the Instructor Dashboard.

On the Instructor Dashboard, click **Student Admin**, and then scroll to the
**Entrance Exam Grade Adjustment** section. The following options are
available.

* **Reset Student Attempts**: Reset the value for one particular student's
  attempts back to zero so that the student can begin work over again. For more
  information, see :ref:`reset_attempts`.

* **Rescore Student Submission**: Rescore the responses that a student has
  submitted. For more information, see :ref:`rescore`.

* **Delete Student State for Problem**: Delete a student's entire history for
  the exam from the database. For more information, see :ref:`delete_state`.

Another option on the Instructor Dashboard is **Show Background Task History
for Student**. If you reset student attempts, rescore student submissions, or
delete student state, the operation runs in the background. If you want to see
a record of all the operations that have run for the entrance exam, select
**Show Background Task History for Student**.

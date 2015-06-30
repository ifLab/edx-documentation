.. _Providing a Course Overview:

#####################################
提供课程概述
#####################################


**********
概览
**********

意向加入课程的学生需要关于课程的具体信息。
包括课程内容，每周计划学习时间，以及课程是否对基础知识和技能有要求。
您将在Studio中明确这些信息。

更多信息请参阅以下主题内容：

* :ref:`Describe Your Course`
* :ref:`Add a Course Image`
* :ref:`Add a Course Video`
* :ref:`Set Course Time Requirements`
* :ref:`Set Course Prerequisites`
* :ref:`Set Important Dates for Your Course`

这些信息大多显示在课程概要页面上，又称课程总结页面。
以下图片是一个典型的课程概要页面。

.. image:: ../../../shared/building_and_running_chapters/Images/about_page.png
 :width: 600
 :alt: An image of the course About page showing the course start and end dates,
     prerequisites, description, and other information

学生注册课程时将看到课程概要页面。注册之后，学生可以在课程面板中看到该课程的详细信息。

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard.png
 :width: 600
 :alt: An image of the dashboard showing courses with start and end dates

.. note:: 如果您的课程将出现在edX.org上，您必须与您的edX项目经理一起准备您的课程概要页面内容。
 包括课程概览，图片和视频。更多信息请参阅`edX101 <https://www.edx.org/course/overview-creating-edx-course-edx-edx101#.VLA9IWTF-RU>`_. 中的 `About
 page lesson <https://www.edx.org/course/overview- creating-edx-course-edx-
 edx101#.VLA9IWTF-RU>`_ 一节。


.. _Describe Your Course:

*********************************
描述您的课程
*********************************

您将在课程概述中描述您的课程。有兴趣参与此课程的学生应该能在概述中得到关于课程的有用信息。
概述中介绍课程的主要思想和描述课程涉及的主题以及概念。
您也可以在概述中说明课程所需预备知识和技能，以便学生能够在课程中有所收获，同时可以提供课程要求和教员信息。

以下是课程概述页面中的课程描述。

.. image:: ../../../shared/building_and_running_chapters/Images/about-page-course-description.png
 :width: 600
 :alt: Image of a course About page with the overview circled

您将通过HTML语言将课程描述输入Studio。 Studio的 **课程描述** 框中有一个包含占位符的模板。

如何添加描述内容

#. 从设置栏中选择 **时间表和详情**
#. 从上至下滚动介绍课程内容，然后找到课程概况位置

  .. image:: ../../../shared/building_and_running_chapters/Images/course_overview.png
   :width: 600
   :alt: Image of the HTML course description.

3. 根据需要，依据模版文本重写课程内容。
   Studio将自动保存您的修改。

   .. note::不要编辑超文本标记语言（HTML）的标签。这些标签匹配课程概述页面的内容。
 
4. 点击文本下方的课程总结页面，检测学生如何看到课程描述。

   修改时请注意，您也许需要等待自动保存完成后才能看到修改后的页面。


.. _Add a Course Image:

************************
添加课程相关图片
************************

您需要为您的课程提供图片。
您向Studio上传添加的相关课程图片会呈现在学生使用界面里。
此图片同样也会呈现在该课程概要页面上。

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard-course-image.png
 :width: 600
 :alt: Image of the course image in the student dashboard

课程图片像素至少为660*240（宽*高），格式应为.JPG或.PNG。

遵循以下步骤添加课程图片：

#. 在 **设置** 菜单中选择 **时间表与详情** 。
#. 向下滚动找到 **课程图片** 一栏。
#. 从您的本地计算机中选择一张图片，点击 **上传课程图片** ，
   然后按照提示找到并上传您的图片。
#. 浏览您的使用界面，并查看如何向学生显示该图片。

.. _Add a Course Video:

*********************************
添加课程视频简介
*********************************

为吸引潜在的学生前来注册，您可以为课程添加视频简介。
视频应展示该课程讲师的部分授课风格

.. image:: ../../../shared/building_and_running_chapters/Images/about-page-course-video.png
 :alt: Image of the course video in the course About page.

视频应回答下列重要问题：

* 谁将讲授这门课程？
* 这门课程隶属哪所大学或学院？
* 这门课程涵盖哪些主题及知识概念？
* 学生为什么要注册学习此门课程？

上传的视频简介应尽可能地简明传达您的信息，且时长至少为两分钟。

确保您的视频简介符合 :ref:`Compression
Specifications` 和 :ref:`Video Formats` 

视频简介添加步骤：


#. 上传课程视频至YouTube视频网站。
   记录网址上 **watch?v =** 到 **&feature** 的中间部分。如下列样例绿框中出现的代码。
   

  .. image:: ../../../shared/building_and_running_chapters/Images/image127.png
    :alt: Image of a sample course video
    
2. 在导览列上，点击设置之后，点击时程表与课程介绍。
#. 向下滚动鼠标至课程视频简介区块。
#. 在视频框下方栏位，输入YouTube视频ID（即步骤一中复制的代码）。
   在您添加代码后，视频将自动装载至视频框中。Stidio将自动保存您的变更。

.. _Set Course Time Requirements:

************************************
设置课程时间需求
************************************

课程一周大概所需时间将显示在课程概要页面底部。
遵循以下步骤设置课程时间需求：

#. 点击设置之后，点击时程表与课程介绍。
#. 下滑鼠标至课程需求。
#. 在一周课程所需时间一栏内，输入您期望学生每周学习此门课程的小时数。
#. 浏览您的课程概要页面，查看如何向学生展示该时间量。


.. _Set Course Prerequisites:

********************************************
设置课程预备知识
********************************************

您可能希望确认学生在上课之前具备特定的基础知识和技能。
为了满足您在课程概述中描述的一般要求，您可以要求学生 :ref:`complete specific prerequisite courses<Specify Prerequisite Courses>` 或者 :ref:`take an entrance exam<Require an Entrance Exam>` ，或两项同时进行。

.. _Specify Prerequisite Courses:

===================================
指定预备知识课程
===================================

您可以要求学生在注册您的课程之前修过特定的edX课程。
学生可以在课程概述页面中看到本课程预备知识相关信息。

.. image:: ../../../shared/building_and_running_chapters/Images/PrereqAboutPage.png
  :width: 500
  :alt: A course About page with prerequisite course information circled

没有完成预备知识课程的学生仍可以注册您的课程并在学生课程面板中查看课程。
但是，与其他课程有所不同，学生课程面板不会显示课件链接。
学生课程面板中将包含预备知识课程概述页面的链接。学生可以在这里注册预备知识课程。

.. image:: ../../../shared/building_and_running_chapters/Images/Prereq_StudentDashboard.png
  :width: 500
  :alt: The Student Dashboard with an available course and a course that is
      unavailable because it has a prerequisite


要指定先修课程，您必须是当前课程以及先修课程的作者。

#. 在Studio中打开您的课程。
#. 在 **设置菜单** 中选择 **时间表与详情** 。
#. 在 **时间表与详情** 页面滚动至 **要求** 项。 
#. 在 **先修课程** 下点击下拉列表选择一门课程。
#. 在页面底部点击 **保存修改** 。

.. note:: 目前您只能指定一门先修课程。


.. _Require an Entrance Exam:

===================================
设置入学考试
===================================

您可以要求学生在访问您的课程材料之前通过入学考试。
如果课程含有入学考试，注册该课程的学生只能看到 **课程更新与新闻** 页面和 **入学考试** 标签，
直到他们通过入学考试。

.. image:: ../../../shared/building_and_running_chapters/Images/EntEx_LandingPage.png
  :width: 500
  :alt: The Entrance Exam page with the first problem visible

学生通过入学考试以后，他们可以访问所有已发布的课程资料。

按照以下步骤设置入学考试。

#. 在Studio中打开您的课程。
#. 在 **设置** 菜单中选择 **日程表与细节** 。 
#. 在 **日程表与细节** 页面下滚到 **要求** 部分。 
#. 选择 **要求学生访问课程资料之前通过入学考试** 。 
#. 在页面底端选择 **保存修改** 。

保存修改之后，Studio自动在您的课程大纲创建 **入学考试** 一节。
去课程大纲添加入学考试内容。

入学考试最佳实践
********************************************

我们强烈建议您遵循以下指导步骤帮助您的学生在入学考试中有良好的体验。

* 确保您的贝塔测试员测试入学考试。

* 确保您在课程信息页面中说明此课程需要入学考试。
  否则学生在注册您的课程并尝试访问课程内容之前不知道需要入学考试。

* 在您的课程信息页面或课程e-mail中，包含关于
  在  `edX Guide for Students <http://doroob-student- documentation.readthedocs.org/en/latest/index.html>`_.
  中
  `entrance exams <http://doroob-student-documentation.readthedocs.org/en/latest/SFD_prerequisites.html#entrance-exam>`_ 
  的信息


在课程大纲里创建入学考试
**************************************************

您将在Studio的课程大纲中创建入学考试。
创建入学考试的步骤与创建其他内容相同。
更多信息请参阅 :ref:`Creating Course Content Index`.

允许学生不参加入学考试
**************************************************

您可以允许学生不参加入学考试。
您需要学生的用户名和注册的邮箱地址。

#. 在导师面板中点击 **学生管理** 。
#. 在 **入学考试调整** 部分输入学生信息。 
#. 在 **学生入学考试选项** 下选择 **允许学生跳过入学考试** 。


调整学生的入学考试
********************************************

如果您在学生参加入学考试之后发现错误，且必须修改考试内容，您可以通过几个选项为学生重新评分。
这些选项可以在教师面板中设置。

.. note:: 每次只能调整一个学生的考试。

在教师面板中，点击 **学生管理** ，滚动至 **调整入学考试成绩** 一栏。
以下选项可供设置。


* **重置学生尝试次数**: 为特定学生重置尝试次数为0，学生可以从头开始答题。
  更多信息请参考 :ref:`reset_attempts`.

* **为学生提交答案重新评分**: 为学生提交的答案重新评分。
  更多信息请参考 :ref:`rescore`.

* **删除学生的问题状态**: 从考试数据库中删除学生的所有历史记录。
  更多信息请参考 :ref:`delete_state` 和 :ref:`Adjust_grades` 

导师面板中的另一个选项是 **查看学生后台测试历史**。
如果您重置了学生的尝试次数，为学生提交的答案重新评分，或者删除学生的状态，
操作将在后台运行。如果您想查看入学考试中进行的所有操作记录，选择**查看学生后台测试历史** 。


.. _Set Important Dates for Your Course:

***********************************
为课程设置重要日期
***********************************

You must set dates and times for enrollment and for the course.

#. In Studio, from the **Settings** menu, select **Schedule and Details**.  
#. Follow the on-screen text to enter the course and enrollment schedule.

   .. image:: ../../../shared/building_and_running_chapters/Images/schedule.png
    :width: 450
    :alt: An image of the course schedule page.


.. note:: The **Time** fields on this page, and the times that students 
 see, use Universal Coordinated Time (UTC).

.. _The Course Start Date:

=======================
课程开始时间
=======================


.. note:: 默认情况下，课程开始时间为 **01/01/2030** ，
以确保课程不会在您希望设定的时间之前开始。
您必须将默认日期修改为您的课程开始的正确日期。

Students see the course start date and time on their **Current Courses**
dashboards and on the course About page. 学生可以在课程开始之前看到课程的某些部分。
例如，他们可以看到您的 **课程信息** 页面，一旦注册本课程以后，他们可以看到课内讨论主题。
更多信息请参阅 :ref:`Create
CourseWide Discussion Topics` 。

The following example shows the course start date and time on the course About
page:

.. image:: ../../../shared/building_and_running_chapters/Images/about-page-course-start.png
 :width: 600
 :alt: An image of the course About page, with the start date circled.

In the dashboard, students see the start dates and times for each of their
courses, as in the following examples.

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard-course-to-start.png
 :width: 600
 :alt: An image of two courses in the student dashboard, with the start dates
     and times circled.

.. note:: If you do not specify a start time for your course, students see
   the default start time, 00:00 Coordinated Universal Time (UTC).


.. _Set the Advertised Start Date:

======================================
设置显示开始日期
======================================

您能设置显示开始日期，这与时间表和详情页面的设置课程开始日期不同。
您若对准确的开始日期不确定，可能会想要这样做。
例如，您可以将开始日期显示成 **2015年春季** 。

设置显示开始日期：

#. 从设置栏中选择高级设置
#. 找到显示开始的关键按键，默认值为零。
#. 输入您想显示的开始日期。您能使用任何字符，附上双引号。若您想将字符格式化为日期，
   （例如，格式化为 02/01/2014），其值就被语法化，呈现给学生的是日期。

  .. image:: ../../../shared/building_and_running_chapters/Images/advertised_start.png
   :alt: Image of the advertised start date policy key with a value of "anytime,
       self-paced"

4. 在本页的末尾点击保存改动

The start date shown on the dashboard is now the value of the **Course
Advertised Start Date** policy key:

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard-course_adver_start.png
 :width: 600
 :alt: An image of a course listing in the student dashboard, with the
     advertised start date circled.

如果您没有更改默认开始日期(01/01/2030)，**课程显示开始日期** 将为空值。
课程面板将不会显示该课程的开始日期。学生只能看到目前课程未开始状态。

.. _The Course End Date:

=====================
The Course End Date
=====================

The course end date is the date after which students can no longer earn credit
toward certificates. Students who have earned certificates can view them after
the course end date.

.. important::
 If you do not set a course end date, students will not be able to access
 earned certificates.

After grades and certificates are finalized, students see the course end date
on their personal **Current Courses** dashboards, as shown in the following
examples.

* If grades and certificates are not yet finalized, students can see the course
  end date and a message:

  .. image:: ../../../shared/building_and_running_chapters/Images/dashboard-wrapping-course.png
   :alt: Image of a course on the student dashboard that has ended, but not
     been graded

* When grades and certificates are finalized, students who have not earned a
  certificate see their score and the score required to earn a certificate:
  
  .. image:: ../../../shared/building_and_running_chapters/Images/dashboard-no-cert-course.png
   :alt: Image of a course on the student dashboard that has ended, but not
     been graded

* Students whose final score is equal to or higher than the required score can
  click **Download Certificate** to get their certificates as PDFs:

  .. image:: ../../../shared/building_and_running_chapters/Images/dashboard-completed-course.png
   :alt: Image of a course on the student dashboard that has ended, but not
     been graded


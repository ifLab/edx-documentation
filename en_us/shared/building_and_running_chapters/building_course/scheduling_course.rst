.. _Scheduling Your Course:

##############################
设置开始和结束日期
##############################

课程以及注册开始日期和结束日期对未来学生和已注册学生都是非常重要的。
注册开始以后，期望加入该课程的学生可以在edX课程目录中看到课程总结页面，然后加入该课程。
已注册学生将在学生界面中看到课程的开始日期。

更多关于课程开始和结束日期的信息，以及日期设置指南，请参阅以下主题。

* :ref:`View Start and End Dates`
* :ref:`Determine Start and End Dates`
* :ref:`Set Start and End Dates`

.. _View Start and End Dates:

***************************************
学生视角查看起止日期
***************************************

.. 或者 “学生查看起止日期视角”？

如果课程还未开始或正在进行，未来学生和现有学生都能看到课程起始日期。
课程结束日期仅在课程结束以后对已注册学生可见。 

未注册本课程的学生可以在课程总结页面中查看课程开始日期。 

.. image:: ../../../shared/building_and_running_chapters/Images/about-page-course-start.png
 :alt: The course About page, showing the start date.
 :width: 600

注册参加课程的学生可以在学生界面中看到课程的开始或结束日期。
这取决于课程是否已经结束。如果课程未开始或在进程中，学生将看到开始日期。
如果课程已经结束了，学生则看到结束日期。

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard-course-start-and-end.png
 :alt: The student dashboard with one course not started, one in progress, and one ended.
 :width: 600

.. _Determine Start and End Dates:

*******************************************
确定起止日期
*******************************************

EdX建议您认真考虑课程的注册起始日期和结束日期。
在您决定了日期以后，您将在Studio中的 **日程与细节**页面中设定日期。
EdX建议您在计划开始课程前一周确认所有重要日期。

.. note::
  您必须与您的edX项目经理就edX.org网页上的课程开始日期进行交流，以确保课程总结页面的日期是正确的。

============================
课程开始时间
============================

课程开始时间决定学生何时能进入已发布的课程内容。
默认情况下，课程开始时间为 **01/01/2030** **00:00 UTC** 
以确保课程不会在您希望设定的时间之前开始。
您必须将默认日期修改为您的课程开始的正确日期。

EdX推荐您将课程开始时间设置为一天中较早的时间，一般设置为00:00 UTC之前。
学生常希望课程在自己的时区内已经开始，并尝试在开始日期中进入课程。
如果您没有指定课程起始时间，学生将会看到默认的时间：格林尼治时间 (UTC)00:00。

学生可以在课程开始之前看到课程的某些部分。
例如，他们可以看到您的 **课程信息** 页面，一旦注册本课程以后，他们可以看到课内讨论主题。
更多信息请参阅 :ref:`Create
CourseWide Discussion Topics` 。

.. note:: 
  您可以为您的课程设置广告日期，这与时间表和详情页面的设置课程开始日期不同。
  您若对准确的开始日期不确定，可能会想要这样做。
  例如，您可以将开始日期显示成2014年春季。
  更多信息请参阅 :ref:`Advertise a Different Start Date`。

============================
课程结束时间
============================

学生修的学分达到获得修课证书要求，课程就该结束了。
结束之后学生可以继续完成课程，但是不能在结束之后获得证书。
课程结束之后，获得修课证书的学生能够审视自己。

.. important:: 
  您若没有设置课程结束日期，学生将不能获得修课证书。

===============================
注册起始时间
===============================

注册起始时间指定了何时学生可以开始注册该课程。
请确保注册起始时间足够提前，让学生能够注册并为课程做好准备。

.. _Enrollment End Date and Time:

===============================
注册结束时间
===============================

注册结束时间指定了何时学生不能再注册本课程。
请确保注册时间充足，让学生能够参加本课程。
注册结束时间不能晚于课程结束时间。

.. important:: 
  For partner courses on edx.org, when the enrollment end date passes,
  the course is no longer listed in the course catalog. EdX encourages you to
  keep enrollment open as long as possible. For more information, contact your
  edX program manager.

.. _Set Start and End Dates:

*******************************************
Set Course and Enrollment Dates and Times
*******************************************

You set dates and times for the course and for course enrollment in Studio.

#. From the **Settings** menu, select **Schedule and Details**.

#. Locate the **Course Schedule** section of the **Schedule & Details** page,
   and replace the placeholder dates and times with your own information.

   When you make changes, a **Save Changes** button appears in the lower right
   corner of the page.

#. When you finish entering your dates and times, select **Save Changes**.

.. note:: 
 The Time fields on this page, and the times that learners see, use Universal
 Coordinated Time (UTC).

EdX recommends that you verify that all important dates are correct one week
before you plan to start the course.

.. _Advertise a Different Start Date:

====================================
Advertise a Different Start Date
====================================

You can advertise a start date for your course that is different from the
course start date you set in the **Schedule and Details** page. You might want
to do this if there is uncertainty about the exact start date. For example, you
could advertise the start date as **Spring, 2015**.

To set an advertised start date in Studio, follow these steps.

#. From the **Settings** menu, select **Advanced Settings**.
#. Find the **Course Advertised Start Date** policy key. The default value is
   **null**.
#. Enter the value you want to display as the advertised start date. You can
   use any string, enclosed in double quotation marks. If you format the string
   as a date (for example, as 02/01/2015), the value is parsed and presented to
   learners as as a date.

  .. image:: ../../../shared/building_and_running_chapters/Images/advertised_start.png
   :alt: Image of the advertised start date policy key with a value of "anytime, self-paced".
   :width: 600

4. Select **Save Changes** at the bottom of the page.

Learners now see the value of the **Course Advertised Start Date** policy key
as the course start date on their dashboards.

If you do not change the default course start date (01/01/2030), and the
**Course Advertised Start Date** policy value is ``null``, then the 
dashboard does not list a start date for the course. Learners just see that
the course has not yet started.

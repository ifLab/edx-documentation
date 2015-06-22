.. _Setting Details About Your Course:

######################################################
设置课程细节
######################################################

此章讲述如何在Studio中设置您的课程细节。
您所设置的细节内容将会影响学生面板中看到的信息。
详情请参阅 :ref:`SFD Dashboard Settings Profile`。

.. contents:: Section Contents
  :local:
  :depth: 1

设置重要日期相关内容请参阅 :ref:`Scheduling Your
Course`.

设置课程证书相关内容请参阅 :ref:`Licensing a
Course`.

.. _The Course About Page:

***********************************
课程总结页面
***********************************

下图是总结页面的例子。学生可以在注册之前看到此页面，并且可能在浏览页面内容后决定注册。

.. image:: ../../../shared/building_and_running_chapters/Images/about_page.png
 :alt: An image of the course About page.
 :width: 600

正如此章所讲述的，您通过Studio设置页面内容。

.. _The Learner Dashboard:

***********************************
学生控制面板
***********************************

如果学生注册您的课程，之后课程和课程图片会在控制面板上显示。
学生从控制面板上能点开开始的课程。
正如 :ref:`Scheduling Your Course` 此章所讲述的，如果课程无法开始，学生能看看开始日期。

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard-course-start-and-end.png
 :width: 600
 :alt: An image of two courses in the dashboard, with the start dates and
     times.

.. _Describe Your Course:

************************
描述您的课程
************************

学生将在您的课程页面中看到您对课程的描述。

例如，课程描述在以下课程总结页面以环形结构展开。

.. image:: ../../../shared/building_and_running_chapters/Images/about-page-course-description.png
 :alt: Image of a course summary with the description circled.
 :width: 600

.. note:: 您必须与您的edX项目经理就edX.org网页上的课程描述进行交流，以确保课程总结页面的内容是正确的。

#. 从设置栏中选择时间表和详情

#. 从上至下滚动介绍课程内容，然后找到课程概况位置

   .. image:: ../../../shared/building_and_running_chapters/Images/course_overview.png
    :alt: Image of the HTML course description.
    :width: 600

#. 根据需要，依据模版文本重写课程内容。不要编辑超文本标记语言（HTML）的标签。
   模版应当包括占位符，请阅览课程概况模版。 :ref:`A Template For Course Overview`
 
#. 点击文本下方的课程总结页面，检测学生如何看到课程描述。

#. 当您修改内容时，**保存修改** 按钮将出现在页面下方。
   完成课程描述后请点击 **保存修改** 按钮。

.. _Add a Course Image:

************************
添加课程相关图片
************************

The course image that you add in Studio appears on the dashboard. It should be
a minimum of 378 pixels in width by 225 pixels in height, and in .jpg or .png
format. Make sure the image that you upload maintains the aspect ratio of those
dimensions so that the image appears correctly on the dashboard.

In the following example, the course image that was added in Studio is circled
in the dashboard.

.. image:: ../../../shared/building_and_running_chapters/Images/dashboard-course-image.png
 :alt: Image of the course image in the dashboard.
 :width: 600

#. From the **Settings** menu, select **Schedule & Details**.

#. Scroll down to the **Course Image** section.

#. To select an image from your computer, click **Upload Course Image**, then
   follow the prompts to find and upload your image.

#. When you make changes, a **Save Changes** button appears at the bottom right
   of the page. Select **Save Changes** when you have added the course image.

#. View your dashboard to test how the image will appear to learners.

.. note:: 
  On edX.org, the course image you add in Studio is used on the learner
  dashboard, but does not automatically appear on the course About page. Work
  directly with your edX program manager to set up the About page assets and
  course image for the course summary page.

.. _Add a Course Video:

*********************************
Add a Course Video
*********************************

The course video appears on the course About page.

In the following example, the course video is circled in the course About
page:

.. image:: ../../../shared/building_and_running_chapters/Images/about-page-course-video.png
 :alt: Image of the course video in the course summary page.
 :width: 600

The course video should excite and entice potential learners to enroll, and
reveal some of the personality the instructors bring to the course.

The video should answer these key questions:

* Who is teaching the course?
* What university or college is the course affiliated with?
* What topics and concepts are covered in your course?
* Why should a learner enroll in your course?

The video should deliver your message as concisely as possible and have a run
time of less than 2 minutes.

Ensure your course introduction video follows the same :ref:`Compression
Specifications` and :ref:`Video Formats` guidelines as course content videos.

#. Upload the course video to YouTube. Make note of the code that appears
   between **watch?v =** and **&feature** in the URL. This code appears in the
   green box below.

   .. image:: ../../../shared/building_and_running_chapters/Images/image127.png
    :alt: Image of a sample course video.
    
#. From the **Settings** menu, select **Schedule & Details**.

#. Scroll down to the **Course Introduction Video** section.

#. In the field below the video box, enter the YouTube video ID (the code you
   copied in step 1). When you add the code, the video automatically loads in
   the video box.

#. When you make changes, a **Save Changes** button appears at the bottom right
   of the page. Select **Save Changes** when you have added the course video.

#. View your course About page to test how the video will appear to learners.

.. note:: 
  On edX.org, you work directly with your Program Manager to set up the course
  video in the summary page.

.. _Set Course Effort Expectations:

*******************************
Set Course Effort Expectations
*******************************

The estimated effort the course requires appears in the course About page. 

You set the hours and minutes a week estimate in Studio.

#. From the **Settings** menu, select **Schedule & Details**.

#. Scroll down to the **Requirements** section.

#. In the **Hours of Effort per Week** field, enter the number of hours you
   expect learners to work on this course each week.

#. When you make changes, a **Save Changes** button appears at the bottom right
   of the page. Select **Save Changes** when you have added the estimated
   effort.

#. View your course About page to test how the requirements will appear to
   learners.

.. _A Template For Course Overview:

************************************************
 A Template For Your Course Overview
************************************************

Replace the placeholders in the following template with your information.

.. code-block:: html

  <section class="about">
    <h2>About This Course</h2>
    <p>Include your long course description here. The long course description 
    should contain 150-400 words.</p>
    <p>This is paragraph 2 of the long course description. Add more paragraphs 
    as needed. Make sure to enclose them in paragraph tags.</p>
  </section>
  <section class="prerequisites">
    <h2>Requirements</h2>
    <p>Add information about the skills and knowledge students need to take 
    this course.</p>
  </section>
  <section class="course-staff">
    <h2>Course Staff</h2>
    <article class="teacher">
      <div class="teacher-image">
        <img src="/static/images/placeholder-faculty.png" align="left" 
        style="margin:0 20 px 0" alt="Course Staff Image #1">
      </div>
      <h3>Staff Member #1</h3>
      <p>Biography of instructor/staff member #1</p>
    </article>
    <article class="teacher">
      <div class="teacher-image">
        <img src="/static/images/placeholder-faculty.png" align="left" 
        style="margin:0 20 px 0" alt="Course Staff Image #2">
      </div>
      <h3>Staff Member #2</h3>
      <p>Biography of instructor/staff member #2</p>
    </article>
  </section>
  <section class="faq">
    <section class="responses">
      <h2>Frequently Asked Questions</h2>
      <article class="response">
        <h3>Do I need to buy a textbook?</h3>
        <p>No, a free online version of Chemistry: Principles, Patterns, and 
        Applications, First Edition by Bruce Averill and Patricia Eldredge 
        will be available, though you can purchase a printed version (
        published by FlatWorld Knowledge) if you’d like.</p>
      </article>
      <article class="response">
        <h3>Question #2</h3>
        <p>Your answer would be displayed here.</p>
      </article>
    </section>
  </section>

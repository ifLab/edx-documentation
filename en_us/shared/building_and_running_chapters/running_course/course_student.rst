.. _Student Data:

############################
学生数据
############################

课程创建后，您可以随时访问学生的数据信息。
请看下面的章节：

.. contents:: Section Contents:
  :local:
  :depth: 2

出于评分原因，您也可以查看学生的个人信息统计表。详见 `Using edX Insights`_.

.. _PII:

***************************************************************
如何维护个人信息
***************************************************************

edX从官网登记用户中收集的个人信息可用于认证、联系及定位。
课程作者有权访问学生的个人信息。

课程工作人员应遵守所在机构制定的规章制度，同时遵守所在地关于个人信息的法律条款，
不得将个人信息外泄，不得盗用他人信息。

.. **Question**: I just made this statement up. What guidance can/should we give, for immediate publication and in the future? (sent to Tena and Jennifer Adams 31 Jan 14)

.. _Access_student_data:

****************************
获取学生数据
****************************

您可以CSV（逗号分隔值）文件格式下载当前参与课程学生的数据。
如果学生人数少于200人，您也可以在教师面板中查看学生数据。

======================
学生自主提供的信息
======================

当学生注册edX帐户时，会选择一个公开可见的用户名，并提供相关的个人信息。
但这并不是硬性要求，所以不是所有的学生都会提供个人信息的。

 .. image:: ../../../shared/building_and_running_chapters/Images/Registration_page.png
   :alt: Fields that collect student information during registration

然后，学生可根据兴趣注册各种各样的课程，注册后则成为该课程的参与者。

您可以访问课程内所有学生自主提供的个人信息，包括：

* 用户名
* 真实姓名
* 电子邮箱地址
* 出生年月
* 性别
* 教育水平 For more information about the reported values, see
  `auth_userprofile.level_of_education`_ column in the *edX Research Guide*.
* 邮件地址
* 学习期望

程工作人员可访问的个人信息永远只包括当前参与课程的学生。
学生可以在课程招生日期内注册您的课程，也可以随时退出课程。
他们也可以随时更改电子邮箱地址和真实姓名。
所以，您可以定时查看这些信息，掌握学生人数变化趋势。

.. note:: 以后的更新中，edX可能会要求学生选择自己的语言和所在地。目前的版本尚未执行。

.. _View and download student data:

==========================================
下载或查看学生数据
==========================================

您可在特定时间段下载学生个人信息报告，了解学生人数情况，
并通过不同时期内学生人数的比较绘制学生人数变化趋势图。
对于分队课程而言，这份个人信息报告也会包括学生的分队情况。

当您选择下载学生数据时，edX服务器会创建一个下载进程。
课程内学生的数量，以及课程是否包含分队功能将决定下载时间长短。
您可以在下载完毕后将学生信息简报保存为CSV格式。

如果课程学生人数少于200人，您可以在教师面板中查看学生数据。

.. note:: 除了学生数据外，您还可以查看课程员工的数据信息。

To download student data, follow these steps.

#. View the live version of your course.

#. Click **Instructor**, then click **Data Download**.

#. To download data about enrolled students in a CSV file, click **Download
   profile information as a CSV**.

  A status message indicates that report generation is in progress. This
  process can take some time to complete, but you can navigate away from this
  page and do other work while it runs.

  To track the progress of the report process, reload the page in your browser
  and scroll down to the **Pending Instructor Tasks** section.

4. To open or save a student data report, click the
   ``{course_id}_student_profile_info_{date}.csv`` file name at the bottom of
   the page.

  All student-supplied data is included in this file without truncation.

To view student data, follow these steps.

.. note:: This option is available only for courses with an enrollment of less 
 than 200.

#. View the live version of your course.

#. Click **Instructor**, then click **Data Download**.

#. To display data about enrolled students, click **List enrolled students'
   profile information**. 

   A table of the student data displays, with one row for each enrolled
   student. Longer values, such as student goals, are truncated.

 .. image:: ../../../shared/building_and_running_chapters/Images/StudentData_Table.png
  :alt: Table with columns for the collected data points and rows for each 
        student on the Instructor Dashboard

For courses that have the cohorts feature enabled, this report also includes a
Cohort column with each student's assigned cohort group.

.. note:: The columns for language and location are included in this report 
 for backward compatibility only. This data is no longer collected during
 student registration.

.. _Access_anonymized:

********************************
Accessing Anonymized Student IDs
********************************

Some of the tools that are available for use with the edX platform, including
external graders and surveys, work with anonymized student data. If it becomes
necessary for you to deanonymize previously anonymized data, you can download a
CSV file to use for that purpose.

To download a file of assigned user IDs and anonymized user IDs:

#. View the live version of your course.

#. Click **Instructor**, then click **Data Download**.

#. Click **Get Student Anonymized IDs CSV**.

You are prompted to open or save the {course-id}-anon-id.csv file for your
course. This file contains the user ID that is assigned to each student at
registration and its corresponding edX-wide anonymized user ID and course
specific anonymized user ID. Values are included for every student who ever
enrolled for your course.

To research and deanonymize student data, you can use this file together with
the ``{course_id}_student_profile_info_{date}.csv`` file of student data or the
``{course_id}_grade_report_{date}.csv`` file of grades.

.. only:: Open_edX

    .. include:: ../../../shared/building_and_running_chapters/running_course/Section_course_student.rst

.. only:: Partners

    .. include:: ../../../shared/building_and_running_chapters/running_course/Section_track_student_activity.rst

.. _Using edX Insights: http://edx-insights.readthedocs.org/en/latest/
.. _auth_userprofile.level_of_education: http://edx.readthedocs.org/projects/devdata/en/latest/internal_data_formats/sql_schema.html#level-of-education

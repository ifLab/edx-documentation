.. _Student Data:

############################
学生数据
############################

课程创建后，您可以随时访问学生的数据信息。
请看下面的章节：

.. contents:: 内容包括:
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

如何下载学生数据：

#. 查看课程现况

#. 单击 **导师** → **数据下载**

#. 如果要下载CSV格式的文件，请单击 **将信息简报保存为CSV文件**

  此时会出现提示消息，显示下载正在进行中。
  这个过程可能要持续一段时间，但是在等待过程中您可以跳到其他页面，干别的事情。
  
  如果想查看下载进度，可以在浏览器中重新加载页面，将滚动条拖至 **正在进行的教师任务** 区域。

4. 单击页面底部的
   ``{course_id}_student_profile_info_{date}.csv`` 文件名，打开或保存学生信息简报

  该文件包含所有学生提供的数据信息。

如何查看学生数据：

.. note:: 仅当学生人数少于200时才可选择此功能。

#. 查看课程现况

#. 单击 **导师** → **数据下载**

#. 单击 **列出学生信息简报** 查看学生数据

   此时会打开一张学生数据表，每一行代表一个学生。比较长的内容，比如学习期望等，只能看见前几句话。
   

 .. image:: ../../../shared/building_and_running_chapters/Images/StudentData_Table.png
  :alt: Table with columns for the collected data points and rows for each 
        student on the Instructor Dashboard

如果该课程启用了分队功能，则会增加“分队”栏，显示学生的分队情况。

.. note:: 为保持向后兼容性，本报告包含“语言”和“所在地”栏。但在学生注册过程中，不会显示这两项。

.. _Access_anonymized:

********************************
获取解析后的学生ID
********************************

edX平台的某些插件，比如外挂评分工具和调查工具，需要提供解析后的学生数据。
如果您需要解析之前加密的数据，可以下载一个CSV文件。

如何下载指定用户ID和匿名用户ID文件：

#. 查看课程现况

#. 单击 **导师** → **数据下载**

#. 单击 **获取学生匿名ID的CSV** 。

此时您需要打开或保存课程的{course-id}-anon-id.csv文件。
该文件包含了学生注册时系统自动分配的ID、edX范围内的匿名ID以及某课程范围内的匿名ID。
只要是曾经参加过课程的学生，都拥有这三个ID。

您可将这个CSV文件与  ``{course_id}_student_profile_info_{date}.csv`` 学生数据文件、
``{course_id}_grade_report_{date}.csv`` 学生成绩文件配合起来使用，
达到解析学生数据的目的。

.. only:: Open_edX

    .. include:: ../../../shared/building_and_running_chapters/running_course/Section_course_student.rst

.. only:: Partners

    .. include:: ../../../shared/building_and_running_chapters/running_course/Section_track_student_activity.rst

.. _Using edX Insights: http://edx-insights.readthedocs.org/en/latest/
.. _auth_userprofile.level_of_education: http://edx.readthedocs.org/projects/devdata/en/latest/internal_data_formats/sql_schema.html#level-of-education

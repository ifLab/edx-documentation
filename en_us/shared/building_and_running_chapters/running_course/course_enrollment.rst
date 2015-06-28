.. _Enrollment:

##########################
招生
##########################

课程编写者和导师可以招收学生、查看课程参与人数以及，在必要的情况下，从教师控制面板中开除学生。

在规定的招生时间内，学生可自行参与课程。
 ``www.edx.org`` 的课程对所有已注册edX账户的学生公开招生。
其他课程，比如在 ``edge.edx.org`` 网站中的课程，
它们的招生只针对了解课程URL的学生或是其他指定范围的学生。

* :ref:`registration_enrollment`

* :ref:`enroll_student`

* :ref:`view_enrollment_count`

* :ref:`unenroll_student`

关于课程招生的数据可在edX Insights 中查看。
您可以在教师控制面板中查看当前课程的Insights：单击 **导师** ，
然后单击页面标题栏中的链接即可。更多信息请参考 `Using edX Insights`_.

.. _registration_enrollment:

*********************************
注册及招生
*********************************

学生在参与课程之前，需要：

#. 注册用户帐户。需提供有效的电子邮件地址用于登录
   ``www.edx.org``， ``edge.edx.org``或者安装edX平台客户端。
   每个平台的用户帐户均不能相同。

#. 通过邮箱中的激活邮件来激活账户。

只要课程招生日期没过，所有注册并激活账户的学生都可以参加
``www.edx.org`` 中的课程，或者，如果知道课程的URL，也可以参与其他课程。

但是，课程编写者及导师在课程中可以随时添加学生，无论该学生是否注册了用户帐户。

为方便管理工作，所有课程工作人员均必须注册、激活用户帐户，并参加课程。

.. _enroll_student:

*********************************
Enroll Students in a Course
*********************************

You enroll students, and other course staff members, in your course by
supplying their email addresses. After the **Enrollment End Date** for a
course students can no longer enroll themselves; however, you can still
explicitly enroll students.

When you enroll people in a course you have these options:

* **Auto Enroll**. When you choose this option, the people who you enroll do
  not need to complete an explicit course enrollment step. Of the list of email
  addresses that you supply, those that correspond to a registered user account
  are immediately enrolled in the course, and your course displays on the
  **Current Courses** dashboard for those users on log in. Email addresses on
  the list that do not match a registered user account are enrolled as soon as
  that account is registered and activated.

  If you do not select **Auto Enroll**, the people who you enroll must also actively locate your course and enroll themselves in it. These students see the course on their dashboards after they have done so.

* **Notify students by email**. When you choose this option, an email message is
  automatically sent to each of the email addresses that you supply. The message
  includes the name of the course and, for students who are not already
  enrolled, a reminder to use that same email address to enroll.

  An example of the email message that a student received when this option was
  selected during enrollment follows. In this example, the student already had a
  registered and activated edx.org account, and both **Auto Enroll** and
  **Notify students by email** were selected.

  .. image:: ../../../shared/building_and_running_chapters/Images/Course_Enrollment_Email.png
        :alt: Email message inviting a student to enroll in an edx.org course

To enroll students or staff members:

#. View the live version of your course.

#. Click **Instructor**, then click **Membership**. 

#. In the **Batch Enrollment** section of the page, enter the username or email
   address of the student, or enter multiple names or addresses separated by
   commas or new lines.

  You can copy and paste data from a CSV file of email addresses. However,
  note that this feature is better suited to courses with smaller enrollments,
  rather than courses with massive enrollments.

4. To streamline the course enrollment process, leave **Auto Enroll** selected.

#. To send students an email message, leave **Notify students by email**
   selected.

#. Click **Enroll**.

.. _view_enrollment_count:

***************************
View an Enrollment Count
***************************

After you create a course, you can access the total number of people who are
enrolled in it. When you view an enrollment count, note that:

* In addition to students, the enrollment count includes the course author,
  course team members, instructors, and course staff. (To work with a
  course in Studio or the LMS, you must be enrolled in that course.)

* Students can unenroll from courses, and course authors and instructors can
  unenroll students when necessary.

  **Note**: The enrollment count displays the number of currently enrolled
  students and course team staff. It is not a historical count of everyone who
  has ever enrolled in the course.

The total number of current enrollees is shown as the sum of the number of
people who selected each of the certification tracks (verified, audit, or
honor) that are available for your course.

To view the enrollment count for a course:

#. View the live version of your course.

#. Click **Instructor**, then click **Course Info** if necessary. 

  The **Enrollment Information** section of the page that opens shows the
  number of people who are currently enrolled in your course and in each of the
  certification tracks.

You can also view or download a list of the people who are enrolled in the
course. See :ref:`Student Data`.

.. _unenroll_student:

*********************************
Unenroll Students from a Course
*********************************

You can remove students from a course by unenrolling them. To prevent students
from re-enrolling, course enrollment must also be closed. You use Studio to
set the **Enrollment End Date** for the course to a date in the past. See
:ref:`Scheduling Your Course`.

**Note**: Unenrollment does not delete data for a student. An unenrolled
student's state remains in the database and is reinstated if the student does
re-enroll.

To unenroll students, you supply the email addresses of enrolled students. 

#. View the live version of your course.

#. Click **Membership**. 

#. In the **Batch Enrollment** section of the page, enter a username or an email
   address, or multiple names or addresses separated by commas or new lines.

#. To send students an email message, leave **Notify students by email**
   selected.

.. note:: The **Auto Enroll** option has no effect when you click **Unenroll**.

5. Click **Unenroll**. The course is no longer listed on the students'
   **Current Courses** dashboards, and the students can no longer contribute to
   discussions or the wiki or access the courseware.

.. _Using edX Insights: http://edx-insights.readthedocs.org/en/latest/

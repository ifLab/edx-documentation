.. _Enabling and Configuring Cohorts:

############################################
启用、配置分队模式
############################################

If you want to use cohorts in your course, you select a strategy for assigning
your students to cohorts: automated assignment, manual assignment, or a hybrid
approach. For more information, see :ref:`Options for Assigning Students to
Cohorts`.

.. note:: Although you can change the assignment method for cohorts at any time,
   you should have a strategy in mind as you design your course, and only make
   changes to cohorts while the course is running if absolutely necessary.

同时您还需要决定是否将全课堂共享的大讨论改为小规模分队讨论。

当您最终决定了分队策略后，请完成以下配置步骤：

#. :ref:`Enable cohorts<Enable Cohorts>`.

#. 根据您最终的分队策略，您需要：
   
  * :ref:`Implement an automated assignment strategy<Implementing the Automated
    Assignment Strategy>`

  * :ref:`Implement a manual assignment strategy<Implementing the Manual
    Assignment Strategy>` and :ref:`manually assign students<Assign Students to
    Cohorts Manually>` to the cohorts you create

  * :ref:`Use a combination of automated and manual assignment<Hybrid
    Assignment>`

3. 将需要更改的大课题转变为分队课题，如不需要，可忽略此步。
   
  * Course-wide discussion topics are unified by default, but you can specify
    that they are :ref:`divided by cohort<Specify Whether CourseWide Discussion
    Topics are Cohorted>`.

  * Content-specific discussion topics are divided by cohort by default. You do
    not need to take any action if you want :ref:`all content-specific
    discussions<Specify that All ContentSpecific Discussion Topics are
    Cohorted>` to be divided by cohort. You only need to change settings if you
    want to make :ref:`only a few discussion topics divided by cohort<Specify
    Some ContentSpecific Discussion Topics as Cohorted>` and make the remaining
    topics unified.

您需要在Studio和教师指示板上完成这些步骤。

为保证学生的最佳课堂体验，这些步骤应在课程开始日期前就设置妥当。
课程开始后，若您仍需更改分队设置，请参考 :ref:`Altering Cohort Configuration`.


.. _Implementing the Automated Assignment Strategy:

***************************************************
启用分队功能
***************************************************

To implement an automated assignment strategy of students to cohorts, you
:ref:`enable the cohort feature<Enable Cohorts>` for your course, and
:ref:`create cohorts<Add Cohorts>` that have the **Automatic** :ref:`assignment
method<Changing the Assignment Method of a Cohort>`. To add students to these
cohorts, you do not need to take any action: the system automatically and
randomly assigns students to the available automatic cohorts when they first
access any course content or discussion topic.

.. note:: You can :ref:`add students manually<Assign Students to Cohorts
   Manually>` to any cohort, whether it was created as an automated cohort or a
   manual cohort.

For a scenario using an automated assignment strategy, see :ref:`All Automated
Assignment`. For a scenario using a combination of automated and manual
assignment to cohorts, see :ref:`Hybrid Assignment`.


.. _About Auto Cohorts:

=================
自动分队
=================

The first time a student first views any course content, including the course
**Discussion** page or content-specific discussion topics, if she is not already
assigned to a cohort, she is randomly assigned to one of the automated cohorts.
If no automated cohorts exist, the system creates a :ref:`Default Cohort Group`
and assigns the student to this default cohort.

.. note:: The default cohort is created to ensure that every student is assigned
   to a cohort. To avoid having to re-assign students from the default cohort to
   other cohorts, make sure you create the automated cohorts that you want in
   your course before the course starts.


.. _Implementing the Manual Assignment Strategy:

***************************************************
采用手动分组策略
***************************************************

To implement a manual assignment strategy of students to cohorts, you
:ref:`enable the cohort feature<Enable Cohorts>` for your course, and
:ref:`create cohorts<Add Cohorts>` that have the **Manual** :ref:`assignment
method<Changing the Assignment Method of a Cohort>`. To add students to these
cohorts, you manually assign students to the appropriate cohort.

.. note:: 手动分队过程应尽量在课程开始之前完成。
   如果课程开始后继续有学生报名参加，您也应该将新加入的学生分到相应队列中。
   If you need to make
   changes to the way you have configured cohorts while your course is running,
   see :ref:`Altering Cohort Configuration`.

For a scenario using a manual assignment strategy, see :ref:`All Manual
Assignment`. For a scenario using a combination of automated and manual
assignment to cohorts, see :ref:`Hybrid Assignment`.


.. _Enable Cohorts:

*********************************
Enabling Cohorts in your Course
*********************************

To enable cohorts in your course, follow these steps.

#. In the LMS, select **Instructor**, then select **Cohorts**. 

#. Select **Enable Cohorts**.
   
You can now :ref:`add cohorts<Add Cohorts>` to your course.

.. warning:: Be very careful in deciding to enable the cohort feature in a live
   course, because doing so affects the course experience for learners. Learners
   might no longer have access to courseware and discussion topics that were
   previously visible to them.

   If you must make changes to cohort configuration while your course is
   running, be sure you understand the consequences of doing so. For details,
   see :ref:`Altering Cohort Configuration`.

.. _Add Cohorts:

****************
Adding Cohorts
****************

After you enable the cohorts feature for your course, you can add cohorts.

#. In the LMS, select **Instructor**, then select **Cohorts**.

#. 单击“添加队列”

#. 给队列起名字

.. note:: Students can see the name of the cohort they are assigned to. The
   message "This post is visible only to {cohort name}" appears with each post
   in discussion topics that are divided by cohort. See :ref:`Read the Cohort
   Indicator in Posts`.

4. Specify whether students are automatically or manually assigned to this
   cohort.
   
#. Optionally, select **Select a Content Group** to associate the cohort with a
   :ref:`content group<About Content Groups>`. For information about creating
   cohort-specific courseware by associating cohorts with content groups, see
   :ref:`Cohorted Courseware Overview`.

#. 单击“保存”
   
Continue implementing your cohort strategy by creating additional cohorts as
applicable, and specifying the assignment method for each cohort.

.. note:: When your course starts, you must have at least one cohort in your
   course that has automatic assignment. If you have not created at least one
   automated assignment cohort in the course by the time that the first student
   accesses your course content, edX creates a default cohort to which students
   are automatically assigned.

For details about adding students to a cohort by uploading a .csv file, see
:ref:`Assign Students to Cohort Groups by uploading CSV`.

For a report that includes the cohort assignment for every enrolled
student, review the student profile information for your course. See
:ref:`View and download student data`.

.. note:: You cannot delete cohorts, but you can change their names or the way
   in which students are assigned to them. If you need to make changes to the
   way you have configured cohorts while your course is running, see
   :ref:`Altering Cohort Configuration`.
   

.. _Assign Students to Cohorts Manually:

***********************************
Assign Students to Cohorts Manually
***********************************

.. note:: Manual assignments should be as complete as possible before your 
 course starts. If student enrollment continues after your course starts, you
 should continue to assign new students to cohorts. 

#. 查看课程的当前状况。在Studio中单击“查看课程现况”

#. 单击“导师”→“成员”

#. 将滚动条拖到底部的“队列管理”区域

#.  在下拉列表中选择一个队列

#. 在“添加学生”字段后，键入单个或多个学生的用户名或电子邮箱，
   多个用户名和邮箱地址之间用逗号分隔，或另起一行。
   您可以复制CSV文件中的电子邮件地址，粘贴到本字段后。

#. 单击“添加学生”，即可将学生添加至制定手动分队队列。
   此时会出现一条消息，提示本次加入小队的学生人数。
   因为每个学生只能加入一个小队，该消息同时也提示了加入其他小队的学生人数。

如果您需要了解每个学生的分组状况，可以查看学生信息简报。详见 :ref:`View and
download student data`.


.. _Assign Students to Cohort Groups by uploading CSV:

***************************************************
Assign Students to Cohorts by Uploading a .csv File
***************************************************

In addition to assigning students to cohorts by entering usernames or email
addresses directly on the **Cohorts** page in the Instructor Dashboard, you can
also upload a .csv file containing a list of students and the cohorts that you
want to assign them to.

Any assignments to cohorts that you specify in the .csv files you upload
will overwrite or change existing cohort assignments. The configuration of
your cohorts should be complete and stable before your course begins. You
should also complete manual cohort assignments as soon as possible after any
student enrolls, including any enrollments that occur while your course is
running. To understand the effects of changing cohort assignments after your
course has started, see :ref:`Altering Cohort Configuration`.

.. note:: Be aware that the contents of the .csv file are processed row by row,
  from top to bottom, and each row is treated independently. 

  For example, if your .csv file contains conflicting information such as
  Student A being first assigned to Cohort 1, then later in the spreadsheet
  being assigned to Cohort 2, the end result of your .csv upload is that Student
  A is assigned to Cohort 2. However, the upload results file will count Student
  A twice in the "Students Added" count: once when they are added to Cohort 1,
  and again when they are added to Cohort 2. Before submitting a file for
  upload, check it carefully for errors.

The requirements for the .csv file are summarized in this table.

.. list-table::
    :widths: 15 30

    * - **Requirement**
      - **Notes**
    * - Valid .csv file

      - The file must be a properly formatted comma-separated values file: 

        * The file extension is .csv.
        * Every row must have the same number of commas, whether or not there
          are values in each cell. 
    * - File size
      - The file size of .csv files for upload is limited to a maximum of 2MB.               
    * - UTF-8 encoded
      
      - You must save the file with UTF-8 encoding so that Unicode characters
        display correctly. 

        See :ref:`Creating a Unicode Encoded CSV File`.

    * - Header row
      - You must include a header row, with column names that exactly match those 
        specified in "Columns" below.
    * - One or two columns identifying students      
      - You must include at least one column identifying students: 
        either "email" or "username", or both. 

        If both the username and an email address are provided for a student,
        the email address has precedence. 
        
        In other words, if an email address is present, an incorrect or non-
        matching username is ignored.

    * - One column identifying the cohort
            
      - You must include one column named "cohort" to identify the cohort
        to which you are assigning each student.

        The specified cohorts must already exist in Studio.

    * -                        
      - Columns with headings other than "email", "username" and "cohort" are
        ignored.

Follow these steps to assign students to cohorts by uploading a .csv file.
      
#. View the live version of your course. For example, in Studio, click **View
   Live**.

#. Click **Instructor**, then click **Cohorts**. 

#. From the **Select a cohort** list, select the cohort to which you are adding
   students.

#. Click **Assign students to cohorts by uploading a CSV file**, then click
   **Browse** to navigate to the .csv file you want to upload.

#. Click **Upload File and Assign Students**. A status message displays
   above the **Browse** button.

#. Verify your upload results on the **Data Download** page. 

   Under **Reports Available for Download**, locate the link to a .csv file with
   "cohort_results" and the date and time of your upload in the filename. The
   list of available reports is sorted chronologically, with the most recently
   generated files at the top.

The results file provides the following information:  

.. list-table::
    :widths: 15 30

    * - **Column**
      - **Description**
    * - Cohort
      - The name of the cohort to which you are assigning students.
    * - Exists
      - Whether the cohort was found in the system. TRUE/FALSE. 
      
        If the cohort was not found (value is FALSE), no action is taken for students you assigned to that cohort in the .csv file.

    * - Students Added
      - The number of students added to the cohort during the row by row
        processing of the .csv file.             
    * - Students Not Found
      - A list of email addresses or usernames (if email addresses were not
        supplied) of students who could not be matched by either email address
        or username and who were therefore not added to the cohort.
             
For a report that includes the cohort assignment for every enrolled student,
review the student profile information for your course. See :ref:`View and
download student data`.


.. _Creating a Unicode Encoded CSV File:

====================================
Creating a Unicode-encoded .csv File
====================================

Make sure the .csv files that you upload are encoded as UTF-8, so that any
Unicode characters are correctly saved and displayed.

.. note:: Some spreadsheet applications (for example, MS Excel) do not allow you
   to specify encoding when you save a spreadsheet as a .csv file. To ensure that
   you are able to create a .csv file that is UTF-8 encoded, use a spreadsheet
   application such as Google Sheets, LibreOffice, or Apache OpenOffice.


.. _Altering Cohort Configuration:

*************************************************
Altering Cohort Configuration in a Running Course
*************************************************

The configuration of cohorts in your course should be complete and stable before
your course begins. Manual cohort assignments should be completed as soon as
possible after any student enrolls, including any enrollments that occur while
your course is running.

If you decide that you must alter cohort configuration after your course starts
and activity in the course discussion begins, be sure that you understand the
consequences of these actions. 

* :ref:`Changing Student Cohort Assignments`
* :ref:`Renaming a Cohort`
* :ref:`Deleting a Cohort`
* :ref:`Changing the Assignment Method of a Cohort`
* :ref:`Disabling the Cohort Feature`


.. _Changing Student Cohort Assignments:

***************************************************
更改学生分队
***************************************************

当课程开始后，学生上传的内容要么对所有人可见，要么只对某一单独小组可见。
当您更改某个学生的分队后，会出现如下三个现象：

* 该学生能继续看见对所有人可见的内容

* 该学生还能看见对新分组可见的内容

* 仅对该学生之前所在分队可见的内容将对其不再可见

某项内容，以及关于该内容的回复、评论的可见性始终保持不变，
哪怕该内容的作者的已经被分到别的队列，也是如此。
所以，学生有时会看见内容突然“消失”，这是正常现象。

为核实学生分队情况，请您下载您课程的学生简报。如果确实需要作出更改，您需要在教师指示板的“成员”页面中将学生手动分配到各个队列中。
为核实学生分队情况，请您下载您课程的  :ref:`student
profile report<View and download student data>` 。如果确实需要作出更改，
您需要在教师指示板的“成员”页面中 :ref:`assign students<Assign Students to Cohorts Manually>`
或者在.csv文件里 :ref:`upload cohort assignment changes<Assign Students to Cohort Groups by
uploading CSV>` 


.. _Renaming a Cohort:

***************
重新命名队列
***************

您可以更改任何队列的名字。包括系统生成的默认队列。

To rename a cohort, follow these steps.

#. View the live version of your course. For example, in Studio click **View
   Live**.

#. Click **Instructor**, then click **Cohorts**. 

#. From the **Select a cohort** list, select the cohort whose name you want to
   change.

#. On the **Settings** tab, in the **Cohort Name** field, enter a new name for
   the cohort.

#. Click **Save**. The name for the cohort is updated throughout the LMS and the
   courseware, including student-visible views.


.. _Deleting a Cohort:

================
Delete a Cohort
================

You cannot delete cohorts. However, you can :ref:`rename a cohort<Renaming a
Cohort>`, :ref:`change its assignment method<Changing the Assignment Method of a
Cohort>`, or move students to other cohorts.

If you decide that you must alter cohort configuration after your course starts
and learners begin viewing the courseware and discussion topics, be sure that
you understand the consequences of these actions. For more details, see
:ref:`Altering Cohort Configuration`.


.. _Changing the Assignment Method of a Cohort:

******************************************
Changing the Assignment Method of a Cohort
******************************************

Although you can change the assignment method of a cohort at any time after you
create it, you should have a strategy in mind as you design your course, and
only make changes to cohorts while the course is running if absolutely
necessary. Be aware of the implications of changing cohort configuration while
your course is running. For more information, see :ref:`Options for Assigning
Students to Cohorts` and :ref:`Altering Cohort Configuration`.

.. note:: When your course starts, you must have at least one cohort in your
   course that has automatic assignment. If you have not created at least one
   automated assignment cohort in the course by the time that the first student
   accesses your course content, edX creates a default cohort to which students are
   automatically assigned. If the :ref:`Default Group<Default Cohort Group>` is the
   only automated assignment cohort in your course, you cannot change its
   assignment method to **Manual**.

To change the assignment method of a cohort, follow these steps.

#. View the live version of your course. For example, in Studio click **View
   Live**.

#. Click **Instructor**, then click **Cohorts**. 

#. From the **Select a cohort** list, select the cohort whose assignment method
   you want to change.

#. On the **Settings** tab, the current assignment method is selected. Change
   the assignment method by selecting the other option, either **Automatic** or
   **Manual**.

#. Click **Save**. 

   The cohort assignment method is updated. 

.. note:: Changing the cohort assignment method has no effect on students who
   are already assigned to this and other cohorts in your course. Students who
   access the course after you make this change are assigned to cohorts based on
   the new assignment method of this cohort combined with the assignment methods
   of all other cohorts in your course.


.. _Disabling the Cohort Feature:

******************************
Disable Cohorts in Your Course
******************************


.. warning:: Be very careful in deciding to disable the cohort feature if you
   previously had it enabled in a live course, because doing so affects the
   course experience for learners. Courseware and discussion posts that were
   shared only with members of particular cohorts are now visible to all
   learners in the course.

   If you must make changes to the way you have configured cohorts while your
   course is running, be sure you understand the consequences of doing so. For
   details, see :ref:`Altering Cohort Configuration`.


To disable cohorts in your course, follow these steps.

#. In the LMS, select **Instructor**, then select **Cohorts**. 

#. Clear the **Enable Cohorts** option.
   
All course content and discussion posts that were previously divided by cohort
immediately become visible to all students.



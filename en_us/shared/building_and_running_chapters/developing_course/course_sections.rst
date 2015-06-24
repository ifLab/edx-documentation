.. _Developing Course Sections:

###################################
创建课程章节
###################################

创建课程章节之前，您必须了解以下内容：

* `What is a Section?`_
* `Viewing Sections in the Outline`_
* `The Student View of a Section`_
* `Sections and Visibility to Students`_
* `Release Statuses of Sections`_

  
创建章节时需完成的任务:

* `Create a Section`_
* `Change a Section Name`_
* `Set a Section Release Date`_
* `Publish all Units in a Section`_
* `Hide a Section from Students`_
* `Delete a Section`_


****************************
什么是章节？
****************************

章节应是课程目录中的第一级标题。
一个章节可以表示一段时间，一章内容或其他组织形式。
一个章节应包含一个或多个小节。

********************************
在课程大纲中预览章节
********************************

下图显示了大纲中四个收起的章节：

.. image:: ../../../shared/building_and_running_chapters/Images/sections-outline.png
 :alt: Four sections in the outline

******************************
学生界面中的章节
******************************

学生可以在课件库中查看章节，并可以通过展开章节查看全部内容。
如下图所示，方框中有三个章节，其中第三个章节展开了所有的小节内容：

.. image:: ../../../shared/building_and_running_chapters/Images/sections_student.png
 :alt: The students view of the course with two sections circled

************************************************
章节对学生的可见性
************************************************

学生无法看见任何尚未发布或者已过发布期限的章节。

如果出现下列情况，学生仍然可以看见已过发布日期的内容：

* The release date for the subsection that contains that content has passed.
* The unit has been published.
* The unit is not hidden from students.

************************************************
Release Statuses of Sections
************************************************

As an course author, you control the release status of sections.  For the
content of a section to be visible to students, the section must be released.
See the following topics for more information about the possible release
statuses of sections.

* `Unscheduled`_
* `Scheduled`_
* `Released`_
* `Released with Unpublished Changes`_
* `Staff Only Content`_

========================
Unscheduled
========================

If you do not change the :ref:`course start date<Set Start and End Dates>`
default value, ``1/1/2030 00:00:00 UTC``, when you create a new section, its
release date will appear as ``Unscheduled``. When the section release date is
unscheduled, students cannot see any content in that section, regardless of
the publishing status of that content.

If you have modified the course start date, when you create a new section, the
default release date is the course start date.

The following example shows how an unscheduled section displays in the
outline, summarized with a gray bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-unscheduled.png
 :alt: An unscheduled section

To make the content available to students, you must schedule the release date.

==========
Scheduled
==========

A section that is scheduled for release on a future date will not be visible to
students until after the release date. Regardless of the publishing status of
content within the section, the entire section will not visible to students.

The following example shows how a section that is scheduled for release
displays in the outline, summarized with a green bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-future.png
 :alt: An section scheduled to release in the future

The scheduled date must pass for the section to be visible to students.

===========================
Released
===========================

A section that is released is visible to students; however, students see only
subsections within the section that are also released, and units that are
published.

The following example shows how a released section displays in the outline,
summarized with a blue bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-released.png
 :alt: An unscheduled section

==================================
Released with Unpublished Changes
==================================

If you change a unit in a released section but do not publish the changes,
students see the last published version of the modified unit.

The following example shows how a released section with unpublished changes 
displays in the outline, with a yellow bar. The section is expanded to show
the unit with unpublished changes.

.. image:: ../../../shared/building_and_running_chapters/Images/section-unpublished-changes.png
 :alt: A section with unpublished changes

You must publish the unit for students to see the updates.

===========================
Staff Only Content
===========================

A section can contain a unit that is hidden from students and available to
staff only. That unit is not visible to students, regardless of the release
date of the section or subsection.

The following example shows how a section that contains a unit that is hidden
from students displays in the outline, summarized with a black bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-hidden-unit.png
 :alt: A section with a hidden unit 


.. _Create a Section:

****************************
Create a Section
****************************

If you do not change the :ref:`course start date<Set Start and End Dates>`
default value, ``1/1/2030``, when you create a new section, its release date
will be ``Unscheduled``. 

If you have modified the course start date, when you create a new section, the
default release date is the course start date.

.. caution:: 
 If the course start date is in the past, newly created sections are
 immediately visible to students.

To create a new section:

#. Click **New Section** at the top or bottom of the outline: 
   
   .. image:: ../../../shared/building_and_running_chapters/Images/outline-create-section.png
     :alt: The outline with the New Section buttons circled

   A new section appears at the end of the course content, with the section
   name selected.

#. Enter the name for the new section. A descriptive name can help learners
   locate content in the courseware. It can also help you select content when
   you analyze performance in edX Insights.

#. :ref:`Add subsections<Create a Subsection>` to the new section as needed.
   
It is recommended that you :ref:`test course content <Testing Your Course
Content>` as you create new sections.

********************************
Change a Section Name
********************************

To edit a section name, hover over the section name to show the Edit icon.

.. image:: ../../../shared/building_and_running_chapters/Images/section-edit-icon.png
  :alt: The Edit Section Name icon

Click the Edit icon next to the section name. The name field becomes editable.
Enter the new name and tab or click out of the field to save the name.

.. _Set a Section Release Date:

********************************
Set a Section Release Date
********************************

To set the section release date:

#. Click the Settings icon in the section box.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-box.png
    :alt: The section settings icon circled

   The **Settings** dialog box opens.

#. Enter the release date and time for the section.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-release-date.png
    :alt: The section release date settings

#. Click **Save**.

For more information, see :ref:`Release Dates`.

.. _Publish all Units in a Section:

********************************
Publish all Units in a Section
********************************

To publish all new and changed units in a section, click the publish icon in
the box for the section.

.. image:: ../../../shared/building_and_running_chapters/Images/outline-publish-icon-section.png
 :alt: Publishing icon for a section

.. note:: 
 The publish icon only appears when there is new or changed content within the
 section.

See :ref:`Unit Publishing Status` for information about statuses and visibility
to students.


.. _Hide a Section from Students:

********************************
Hide a Section from Students
********************************

You can hide all content in a section from students, regardless of the status
of subsections and units within the section.

For more information, see :ref:`Content Hidden from Students`.

To hide a section from students:

#. Click the Settings icon in the section box.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-box.png
    :alt: The section settings icon circled

   The **Settings** dialog box opens.

#. Check **Hide from students**.

   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-hide.png
    :alt: The section hide from students setting

#. Click **Save**.

Now, no content in the section is visible to students.

To make the section visible to students, repeat these steps and clear the
**Hide from students** check box.

.. warning::
 When you clear the **Hide from students** check box for a section, not all
 content in the section is necessarily made visible to students. If you
 explicitly set a subsection or unit to be hidden from students, it remains
 hidden from students. Unpublished units remain unpublished, and changes to
 published units remain unpublished.

********************************
Delete a Section
********************************

When you delete a section, you delete all subsections and units within the
section.

.. warning::  
 You cannot restore course content after you delete it. To ensure you do not
 delete content you may need later, you can move any unused content to a
 section in your course that you set to never release.

To delete a section:

#. Click the delete icon in the section that you want to delete.

  .. image:: ../../../shared/building_and_running_chapters/Images/section-delete.png
   :alt: The section with Delete icon circled

2. When you receive the confirmation prompt, click **Yes, delete this
   section**.

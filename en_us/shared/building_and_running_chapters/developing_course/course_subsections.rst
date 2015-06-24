.. _Developing Course Subsections:

###################################
构建课程小节
###################################

构建课程小节之前您必须了解以下信息：

* `What is a Subsection?`_
* `Viewing Subsections in the Outline`_
* `The Student View of a Subsection`_
* `Subsections and Visibility to Students`_
* `Release Statuses of Subsections`_
  
小节操作：

* `Create a Subsection`_
* `Change a Subsection Name`_
* `Set a Subsection Release Date`_
* `Set the Assignment Type and Due Date for a Subsection`_
* `Publish all Units in a Subsection`_
* `Hide a Subsection from Students`_
* `Delete a Subsection`_


****************************
什么是小节？
****************************

小节是章节的组成部分，一个小节通常包括一个或多个单元。小节通常代表课程的某个主题，或者其他组织形式。
小节有时也被称为“课”或“学习顺序”。


***********************************
小节在课程大纲中的显示方式
***********************************

下图呈现了三个收起的小节在大纲中的显示方式：

.. image:: ../../../shared/building_and_running_chapters/Images/subsections.png
 :alt: Three collapsed subsections in the outline


*********************************
小节在学生端的呈现样式
*********************************

学生可以在课件库中查看小节，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/subsections_student.png
 :alt: The student view of the outline


************************************************
小节与对学生可见性
************************************************

学生无法观看未设置发布日期及发布日期未到的小节内容。

学生如果想观看已过发布日期的课程内容，必须满足以下三个条件：

* 父章节的发布日期已到。
* 单元发布完成。
* 发布单元没有对学生隐藏。

************************************************
小节发布状态
************************************************

课程制作者能控制小节的发布状态。
只有当小节处于发布状态时，学生才能看见内容。
点击以下链接查看更多信息：

* `Scheduled with the Section`_
* `Unscheduled`_
* `Scheduled Later than the Section`_
* `Scheduled with Unpublished Changes`_
* `Released with Unpublished Changes`_
* `Released`_

==========================
与章节同时发布
==========================

由于课程小节的发布日期默认与章节一致，因此一旦发布章节内容，学生就可以浏览小节中的内容。

下图展示了默认发布日期与所在章节发布日期相同的小节在课程大纲中的显示模式：


.. image:: ../../../shared/building_and_running_chapters/Images/subsection-scheduled.png
 :alt: A subsection scheduled to release with the section


========================
未设置发布日期
========================

如果未设置父章节的发布日期，那么新建的小节也自动默认未设置发布日期。

无论小节中的单元是否发布，学生都无法看见未发布的小节内容。

下图展示了未设置发布日期的小节在大纲中的显示模式：

.. image:: ../../../shared/building_and_running_chapters/Images/subsection-unscheduled.png
 :alt: An unscheduled subsection

除非您设置小节的发布日期，否则学生无法浏览该部分内容。


===================================
晚于章节发布
===================================

小节的发布日期可以晚于章节的发布日期。 

无论小节中的单元是否发布，学生都只有在小节发布日期时才能看见该部分内容。

下图中，小节的发布日期就晚于父章节的发布日期：

.. image:: ../../../shared/building_and_running_chapters/Images/subsection-scheduled-different.png
 :alt: A subsection scheduled to release later than the section

只有在发布日期到了后，学生才能看见该小节的内容。

==================================
Scheduled with Unpublished Changes
==================================

You can make changes to a published unit before its parent subsection
is released. 

In this situation, when the release date for the subsection passes, the last
published version of units within the subsection are made visible to students.
The changes in units are not visible to students until you publish them.

The following example shows how a scheduled subsection with unpublished changes
displays in the outline, summarized with a yellow bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-scheduled-with-changes.png
 :alt: A scheduled subsection with unpublished changes


==================================
Released with Unpublished Changes
==================================

If you modify a unit within a released subsection, those modifications are not
visible to students until you publish them.

The following example shows how a released section that has unpublished changes
displays in the outline, summarized with a yellow bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-released-with-changes.png
 :alt: A released subsection with unpublished changes

===========================
Released
===========================

A subsection that is released is visible to students; however, students see
only units within the subsection that are published.

The following example shows how a released subsection displays in the
outline, summarized with a blue bar.

.. image:: ../../../shared/building_and_running_chapters/Images/subsection-released.png
 :alt: A released subsection

===========================
Staff Only Content
===========================

A subsection can contain a unit that is hidden from students and available to
staff only. That unit is not visible to students, even if the subsection has
been released.

The following example shows how an subsection that contains a unit that is
hidden from students displays in the outline, summarized with a black bar.

.. image:: ../../../shared/building_and_running_chapters/Images/section-hidden-unit.png
 :alt: A section with a hidden unit 

.. _Create a Subsection:

****************************
Create a Subsection
****************************

To create a new subsection:

#. In the outline, expand the section in which you want to create a new
   subsection.
#. Click **New Subsection** at the bottom of the expanded section. A new
   subsection appears at the end of the section, with the subsection name
   selected.
#. Enter the name for the new subsection. A descriptive name can help learners
   locate content in the courseware. It can also help you select content when
   you analyze performance in edX Insights.
#. :ref:`Add units<Create a Unit>` to the new subsection as needed.
   
It is recommended that you :ref:`test course content <Testing Your Course
Content>` as you create new subsections.

********************************
Change a Subsection Name
********************************

To change a subsection name, click the Edit icon next to the subsection name.
The name field becomes editable. Enter the new name and tab or click out of the
field to save the name.

.. _Set a Subsection Release Date:

********************************
Set a Subsection Release Date
********************************

To set the subsection release date:

#. Click the Settings icon in the subsection box.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/subsections-settings-icon.png
    :alt: The subsection settings icon circled

   The **Settings** dialog box opens.

#. Enter the release date and time for the section.

   .. image:: ../../../shared/building_and_running_chapters/Images/subsection-settings-release.png
    :alt: The subsection release date settings

#. Click **Save**.

For more information, see :ref:`Release Dates`.

.. _Set the Assignment Type and Due Date for a Subsection:

********************************************************
Set the Assignment Type and Due Date for a Subsection
********************************************************

You set the assignment type for problems at the subsection level. 

When you set the assignment type for a subsection, all problems within the
subsection are graded and weighted as a single type.  For example, if you
designate the assignment type for a subsection as **Homework**, then all
problem types in that subsection are graded as homework.

To set the assignment type and due date for a subsection:

#. Click the Settings icon in the subsection box.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/subsections-settings-icon.png
    :alt: The subsection settings icon circled

   The Settings dialog box opens.

#. Select the assignment type for this subsection in the **Grade as** field.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/subsection-settings-grading.png
    :alt: The subsection settings with the assignment type and due date circled

#. Enter or select a due date and time for problems in this subsection.
#. Click **Save**.

For more information, see :ref:`Establish a Grading Policy`.

.. _Publish all Units in a Subsection:

**********************************
Publish all Units in a Subsection
**********************************

To publish all new and changed units in a subsection, click the publish icon in
the box for the subsection.

.. image:: ../../../shared/building_and_running_chapters/Images/outline-publish-icon-subsection.png
 :alt: Publishing icon for a subsection

.. note:: 
 The publish icon only appears when there is new or changed content within the
 subsection.

See :ref:`Unit Publishing Status` for information about statuses and visibility
to students.

.. _Hide a Subsection from Students:

********************************
Hide a Subsection from Students
********************************

You can hide all content in a subsection from students, regardless of the
status of units within the section.

For more information, see :ref:`Content Hidden from Students`.

To hide a subsection from students:

#. Click the Settings icon in the subsection box.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/subsections-settings-icon.png
    :alt: The subsection settings icon circled

   The **Settings** dialog box opens.

#. Check **Hide from students**.

   .. image:: ../../../shared/building_and_running_chapters/Images/subsection-settings-hidden.png
    :alt: The subsection hide from students setting

#. Click **Save**.

Now, no content in the subsection is visible to students.

To make the subsection visible to students, repeat these steps and clear the
**Hide from students** check box.

.. warning::
 When you clear the **Hide from students** check box for a subsection, not all
 content in the subsection is necessarily made visible to students. If you
 explicitly set a unit to be hidden from students, it remains hidden from
 students. Unpublished units remain unpublished, and changes to published units
 remain unpublished.

.. _Delete a Subsection:

********************************
Delete a Subsection
********************************

When you delete a subsection, you delete all units within the subsection.

.. warning::  
 You cannot restore course content after you delete it. To ensure you do not
 delete content you may need later, you can move any unused content to a
 section in your course that you set to never release.

To delete a subsection:

#. Click the delete icon in the subsection that you want to delete.

  .. image:: ../../../shared/building_and_running_chapters/Images/subsection-delete.png
   :alt: The subsection with Delete icon circled

2. When you receive the confirmation prompt, click **Yes, delete this
   subsection**.

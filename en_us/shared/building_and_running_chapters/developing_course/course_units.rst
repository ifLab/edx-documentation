.. _Developing Course Units:

###################################
构建课程单元
###################################

在大纲中创建单元前，请先了解以下信息：

* `What is a Unit?`_
* `Viewing Units in the Outline`_
* `Viewing the Unit Page`_
* `Viewing Units as a Student`_
* `Unit Publishing Status and Visibility to Students`_
* `Unit Publishing Status`_

创建课程单元时，您需要完成以下任务：

* `Create a Unit`_
* `Edit a Unit`_
* `Preview a Unit`_
* `Publish a Unit`_
* `Discard Changes to a Unit`_
* `View a Published Unit`_
* `Hide a Unit from Students`_
* `Delete a Unit`_

您可以通过 :ref:`course components<Developing Course
Components>` 为单元添加内容。

.. _What is a Unit?:

****************************
什么是单元？
****************************

单元是 :ref:`subsection<Developing Course Subsections>` 的组成部分

一个单元通常包含若干个 :ref:`components<Developing Course Components>`,
如 :ref:`HTML content<Working with HTML Components>`、
:ref:`problems<Working with Problem Components>`、 :ref:`discussions<Working
with Discussion Components>`， 和
:ref:`videos<Working with Video Components>`。

****************************
在大纲中查看单元
****************************

在课程大纲中，您可以扩展父章节、小节查看单元内容： :ref:`expand<Navigating the Course Outline>`

.. image:: ../../../shared/building_and_running_chapters/Images/outline-callouts.png
 :alt: An outline with callouts for sections, subsections, and units

****************************
查看单元页面
****************************

在大纲中点击单元名称，即可打开单元页面。如下图

.. image:: ../../../shared/building_and_running_chapters/Images/unit-page.png
 :alt: The Unit page

****************************
Viewing Units as a Student 
****************************

在学习管理系统中，所有小节中的单元都以链接的形式出现在页面上方的课程进度条中，活动单元就在链接下方显示，如下图所示：


.. image:: ../../../shared/building_and_running_chapters/Images/Units_LMS.png
 :alt: Image of units from the student's point of view

.. _The Unit Workflow:

************************************************
单元工作流程
************************************************

当您在课程大纲中完成 :ref:`section<Developing Course Sections>` 和
:ref:`subsection<Developing Course Subsections>` 后，您就可以开始搭建单元。

基本的操作步骤如下：

#. :ref:`Create a new unit<Create a Unit>`.
#. :ref:`Add components to the unit<Add a Component>`.
#. :ref:`Publish the unit<Publish a Unit>`.
   
发布单元后，您可以进行一下操作：

#. :ref:`Modify components in the unit<Developing Course Components>`.
#. :ref:`Publish the changes to the unit<Publish a Unit>`.
   
下图显示了搭建单元的流程：

.. image:: ../../../shared/building_and_running_chapters/Images/workflow-create-unit.png
 :alt: Diagram of the unit development workflow
   
完成以上步骤后，单元的 **发布状态** 就会发生改变。
课程内容是否对学生可见取决于单元的发布状态及
:ref:`release dates<Release Dates>`，详细信息请参看下一节。

.. _Unit States and Visibility to Students:

*************************************************
Unit Publishing Status and Visibility to Students
*************************************************

以下信息总结了学生是否可以查看单元内容的情况：

* 学生无法看见发布状态为 `Draft (Never
  Published)`_的单元。

* 学生无法看见发布状态为 `Visible to Staff
  Only`_。详细信息请查看 `Hide a Unit from Students`_ 。

* 学生无法看见发布状态为 `Published Not Yet
  Released`_ 的单元。 到了发布日期后，该单元的状态会变为 `Published and Live`_。

* 当单元的发布状态为 `Published and Live`_，学生可以查看当前版本的单元内容。
  
* 如果单元的状态为 `Draft (Unpublished Changes)`_，且该单元所在的小节、章节的发布日期已过，那么学生只能看见上一版本的内容。 

详细信息请查看 :ref:`Controlling Content Visibility`.

.. _Unit Publishing Status:

************************************************
单元的发布状态
************************************************ 

课程制作者可以控制课程单元的发布状态：

* `Draft (Never published)`_
* `Published and Live`_
* `Published (not yet released)`_
* `Draft (Unpublished changes)`_
* `Visible to Staff Only`_

.. _Draft (Never Published):

========================
草稿（永不发布）
========================

当您新建一个单元，并添加组件后，这个单元的发布状态会显示为 **Draft (Never Published)**，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-never-published.png
 :alt: Status panel of a unit that has never been published

在Studio中，您可以查看正在搭建的课程内容。当单元的发布状态为“草稿（永不发布）”时，即使发布日期已过，学生也无法查看该内容。

虽然您无法在学习管理系统（LMS）中查看该单元，但是您可以 :ref:`preview the
unit<Preview Course Content>`。

若想让该单元显示在学习管理系统（LMS）中您必须 :ref:`publish the unit<Publish a Unit>` 。

.. _Published and Live:

====================
Published and Live
====================

The release date for the section and subsection have passed. You've published
the unit and haven't made any changes to it. You and students both see the
current version of the unit.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-published.png
 :alt: Status panel of a unit that is published

.. _Published Not Yet Released:

====================================
Published (not yet released)
====================================

You've published the unit, but the release date hasn't passed. Students cannot
see this unit until the release date passes.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-published_unreleased.png
 :alt: Status panel of a unit that is published but not released

.. _Draft (Unpublished Changes):

===========================
Draft (Unpublished changes)
=========================== 

When you edit a published unit, whether or not it is released, the unit's
publishing status changes to **Draft (Unpublished Changes)**, as shown in the
status panel.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-pending-changes.png
 :alt: Status panel of a unit that has pending changes

In Studio, you see the draft of the content that you're working on. If the
release date has passed, students see the last published version of the unit.
If the release date hasn't passed, students can't see your content.

You must :ref:`publish the unit<Publish a Unit>` for students to see your
changes.

You can :ref:`preview the changes to a unit<Preview Course Content>` to test
how your changes will appear to students after you publish the unit.

.. _Visible to Staff Only:

===========================
Visible to Staff Only
===========================

When you :ref:`hide a unit from students<Hide a Unit from Students>`, the
unit's publishing status changes to **Visible to Staff Only**.

The publishing status of a unit can be **Visible to Staff Only** if you hid the
parent :ref:`section<Hide a Section from Students>` or :ref:`subsection<Hide a
Subsection from Students>` from students.

Students never see a unit with this status, even if it has been published and
the release date has passed.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-unpublished.png
 :alt: Status panel of a unit that has pending changes

.. _Create a Unit:

****************************
Create a Unit
****************************

You can create a unit from the outline or create a unit in the same subsection
from the unit page.

To create a unit from the outline:

#. In the outline, expand the subsection in which you want to create a new
   unit.
#. Click **New Unit** at the bottom of the expanded subsection. A new
   page opens for you to add components to the unit.
#. On the unit page, the unit name is selected. Supply an identifying name. A
   descriptive name can help learners locate content in the courseware. It can
   also help you select content when you analyze performance in edX Insights.
#. :ref:`Add components<Add a Component>` to the new unit as needed.

To create a new unit from a unit page:

#. In the **Unit Location** panel, click **New Unit**.

   .. image:: ../../../shared/building_and_running_chapters/Images/unit_location.png
    :alt: The Unit Location panel in the Unit page

   The unit page for the new unit opens automatically.

#. On the unit page, the unit name is selected. Supply an identifying name. A
   descriptive name can help learners locate content in the courseware. It can
   also help you select content when you analyze performance in edX Insights.

#. :ref:`Add components<Add a Component>` to the new unit as needed.

You must then :ref:`publish the unit<Publish a Unit>` to make it visible to
students.


.. _Edit a Unit:

**************
Edit a Unit
**************

You can edit a unit in the following ways.

* `Edit the unit name`_
* :ref:`Develop components<Developing Course Components>`
* `Reorganize Components in Units`_

When you make any of these changes, if you previously published the unit, the
state changes to `Draft (Unpublished Changes)`_. You must then :ref:`publish
the unit<Publish a Unit>` to make your edits visible to students.


==============================
Edit the Unit Name
==============================

To edit a unit name, click the Edit icon next to the name.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-edit-icon.png
  :alt: The Edit Unit Name icon

The name field becomes editable. Enter the new name and then press the Tab key
or click out of the field to save the name.

==============================
Reorganize Components in Units
==============================

You can reorganize components within a unit by dragging and dropping them to
new locations.

To move a component, hover over the handle on the right of the component's box
until the cursor changes to a four-headed arrow. For example, in the image
below, the handle for the discussion component is selected.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-drag-selected.png
  :alt: A discussion component selected to drag it

Then, click and drag the component to the location that you want. 

A dashed outline indicates where the component will land when you release the
mouse button. For example, in the image below, the discussion component is
being moved to the top of the unit.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-drag-moved.png
 :alt: A component being dragged to a new location  

.. _Preview a Unit:

****************************
Preview a Unit
****************************

You preview a unit to review and test the content before it is visible to
students.

You can preview a unit before it is published and before the course is live.
In a live course, after the unit is published and if there are no pending
changes, previewing a unit is exactly the same as viewing the live version of
the unit.

To preview the unit, in the unit page, click **Preview**.

.. image:: ../../../shared/building_and_running_chapters/Images/preview_changes.png
 :alt: A course unit page, with the Preview button circled

The unit opens in preview mode.

.. image:: ../../../shared/building_and_running_chapters/Images/preview_mode.png
 :alt: The unit in preview mode in the LMS

When you are revising a previously published unit, it is helpful to preview
your changes in one window and :ref:`view the published unit<View a Published
Unit>` in a second window.

.. _Publish a Unit:

****************************
Publish a Unit
****************************

Publishing a unit makes the current version of the unit in Studio available to
students, if the release date for the section and subsection have passed.

You publish a unit that has a status of `Draft (Never Published)`_ or `Draft
(Unpublished Changes)`_. When you publish a unit, the status changes to
`Published and Live`_ or `Published Not Yet Released`_.

You can publish a unit from the unit page or the course outline.

=======================================
Use the Unit Page to Publish a Unit
=======================================

To publish the unit, click **Publish** in the status panel:

.. image:: ../../../shared/building_and_running_chapters/Images/unit-publish-button.png
 :alt: Unit status panel with Publish button circled


=======================================
Use the Outline to Publish a Unit
=======================================

To publish a unit from the outline, click the publish icon in the box for the
unit:

.. image:: ../../../shared/building_and_running_chapters/Images/outline-publish-icon-unit.png
 :alt: Publishing icon for a unit

.. note:: 
 The publish icon only appears when there is new or changed content in the
 unit.

.. _Discard Changes to a Unit:

****************************
Discard Changes to a Unit
****************************

When you modify a published unit, your changes are saved in Studio, though the
changes aren't visible to students until you publish the unit again.

In certain situations, you may decide that you never want to publish your
changes. You can discard the changes so that Studio reverts to the last
published version of the unit.

To discard changes and revert the Studio version of the unit to the last
published version, click **Discard Changes** in the status panel.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-discard-changes.png
 :alt: Unit status panel with Discard Changes circled

.. caution::
 When you discard changes to a unit, the changes are permanently deleted. You
 cannot retrieve discarded changes or undo the action.


.. _View a Published Unit:

****************************
View a Published Unit
****************************

To view the last published version of a unit in the LMS, click **View Live
Version**.

.. image:: ../../../shared/building_and_running_chapters/Images/unit_view_live_button.png
 :alt: Unit page with View Live Version button circled

The unit page opens in the LMS in Staff view. You may be prompted to log in to
the LMS.

If the unit status is `Draft (Unpublished Changes)`_, you do not see your
changes in the LMS until you publish the unit again.

If the unit status is `Draft (Never Published)`_, the **View Live Version**
button is not enabled.

.. _Hide a Unit from Students:

****************************
Hide a Unit from Students
****************************

You can prevent students from seeing a unit regardless of the unit status or
the release schedules of the section and subsection. 

For more information, see :ref:`Content Hidden from Students`.

You can hide a unit from students using the course outline or the unit page.

=======================================
Use the Unit Page to Hide a Unit
=======================================

Select the **Hide from students** check box in the status panel.

.. image:: ../../../shared/building_and_running_chapters/Images/unit-hide.png
 :alt: Unit status panel with Hide from Students checked

For more information, see :ref:`Controlling Content Visibility`.

=======================================
Use the Outline to Hide a Unit
=======================================

#. Click the Settings icon in the unit box.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/outline-unit-settings.png
    :alt: The unit settings icon circled

   The **Settings** dialog box opens.

#. Check **Hide from students**.

   .. image:: ../../../shared/building_and_running_chapters/Images/outline-unit-settings-dialog.png
    :alt: The unit hide from students setting

#. Click **Save**.

=======================================
Make a Hidden Unit Visible to Students
=======================================

Before you make a hidden unit visible to students, be aware that course content
will immediately be visible to students, as follows.

* For a hidden unit that previously was published, clearing the check box
  publishes the current content for the unit. If you made changes to the unit
  while is was hidden, those draft changes are published.

* When you make a section or subsection that was previously hidden visible to
  students, draft content in units is *not* published. Changes you made since
  last publishing units are not made visible to students.

You can make a hidden unit visible to students from the unit page or the course
outline. Follow the instructions above and clear the **Hide from students**
check box.

You are prompted to confirm that you want to make the unit visible to students.

********************************
Delete a Unit
********************************

You delete a unit from the course outline.

When you delete a unit, you delete all components within the unit.

.. warning::  
 You cannot restore course content after you delete it. To ensure you do not
 delete content you may need later, you can move any unused content to a
 section in you

To delete a unit:

#. Click the delete icon in the box for the unit you want to delete.

.. image:: ../../../shared/building_and_running_chapters/Images/section-delete.png
 :alt: The section with Delete icon circled

2. When you receive the confirmation prompt, click **Yes, delete this
   unit**.

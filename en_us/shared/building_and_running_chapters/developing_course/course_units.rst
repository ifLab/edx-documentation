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
已发布且可在线观看
====================

当单元所在的章节、小节已到发布日期，且您发布了该单元也没有修改单元内容，那么您和学生都能看见当前版本的内容。

.. image:: ../../../shared/building_and_running_chapters/Images/unit-published.png
 :alt: Status panel of a unit that is published

.. _Published Not Yet Released:

====================================
已发布但尚不可在线观看
====================================

虽然您已经发布了该单元，但是还未到发布日期，所以学生是无法看见该部分内容的。

.. image:: ../../../shared/building_and_running_chapters/Images/unit-published_unreleased.png
 :alt: Status panel of a unit that is published but not released

.. _Draft (Unpublished Changes):

===========================
草稿（尚未发布更改内容）
=========================== 

对已发布的单元进行发布时，无论是否到发布日期，这个单元的发布状态会自动显示为 **草稿（尚未发布更改内容）**，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-pending-changes.png
 :alt: Status panel of a unit that has pending changes

在Studio中，您可以查看正在编辑的单元。如果该单元的发布日期已到，学生可以看见上一次发布的内容，但是，如果发布日期尚未到，学生是无法查看该单元内容的。


只有您 :ref:`publish the unit<Publish a Unit>` 学生才能看见。

您可以 :ref:`preview the changes to a unit<Preview Course Content>` ，以测试该部分内容在发布后是如何在学生端显示的。

.. _Visible to Staff Only:

===========================
仅对教员可见
===========================

当您 :ref:`hide a unit from students<Hide a Unit from Students>`，该单元的发布状态会显示成 **仅对教员显示**。

如果您对学生隐藏单元的父章节或者父小节，该单元的发布状态也会显示为 **仅对教员显示**。

在这种状态下，无论发布日期是否到达，学生都无法查看单元内容的。

.. image:: ../../../shared/building_and_running_chapters/Images/unit-unpublished.png
 :alt: Status panel of a unit that has pending changes

.. _Create a Unit:

****************************
新建单元
****************************

您可以在课程大纲或者单元所在的小节中新建单元。

如何在大纲中创建单元：

#. 在 **课程大纲** 页面，首先扩展您要新建小节的小节。

#. 单击小节下方的 **新建小节** ，如此，一个没有内容的新单元就出现在小节下方。
#. 输入单元名。描述性强的名称能帮助学生在课件中找到相应内容，同时也帮助您在edX Insights中分析绩效时选择内容。
#. 为单元 :ref:`Add components<Add a Component>` 。

如何在单元页面中新建单元

#. 在单元页面，点击 **新建单元** 。

   .. image:: ../../../shared/building_and_running_chapters/Images/unit_location.png
    :alt: The Unit Location panel in the Unit page

   自动弹出新建单元页面。

#. 在单元页面，输入单元名。描述性强的名称能帮助学生在课件中找到相应内容，同时也帮助您在edX Insights中分析绩效时选择内容。

#. 为单元 :ref:`Add components<Add a Component>` 。

只有 :ref:`publish the unit<Publish a Unit>` ，学生才能看见单元内容。


.. _Edit a Unit:

**************
编辑单元
**************

您可以通过以下方式编辑单元：

* `Edit the unit name`_
* :ref:`Develop components<Developing Course Components>`
* `Reorganize Components in Units`_

对单元进行编辑，该单元的发布状态会显示为 `Draft (Unpublished Changes)`_，您必须重新 :ref:`publish
the unit<Publish a Unit>` ，只有这样学生才能看见修改后的内容。


==============================
编辑单元名
==============================

点击单元名旁边的图标以编辑单元名。

.. image:: ../../../shared/building_and_running_chapters/Images/unit-edit-icon.png
  :alt: The Edit Unit Name icon

重新输入单元名称后，保存。

==============================
重组单元组件
==============================

您可以通过拖放和移动组件位置来重组单元内的各个组件。

移动组件时，先将鼠标悬停在组件的右上方直至光标变为“四向箭头”，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-drag-selected.png
  :alt: A discussion component selected to drag it

其次，按住数遍拖动组件至新的位置。

最后，当出现虚线框提示您组件重新安放的位置时，您就可以松开鼠标，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-drag-moved.png
 :alt: A component being dragged to a new location  

.. _Preview a Unit:

****************************
预览单元
****************************

您可以通过预览单元来检测单元内容在学生端的显示样式

You can preview a unit before it is published and before the course is live.
In a live course, after the unit is published and if there are no pending
changes, previewing a unit is exactly the same as viewing the live version of
the unit.

预览单元内容只需在单元页面点击“预览更改”按钮。

.. image:: ../../../shared/building_and_running_chapters/Images/preview_changes.png
 :alt: A course unit page, with the Preview button circled

即会弹出预览窗口，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/preview_mode.png
 :alt: The unit in preview mode in the LMS

编辑已发布单元时，您可以在两个窗口对比更改前和更改后的单元内容。

.. _Publish a Unit:

****************************
发布单元
****************************

如果父章节及小节的发布日期已到，且发布该单元，学生才能看见单元内容。

您可以发布状态为 `Draft (Never Published)`_ 或者 `Draft
(Unpublished Changes)`_的单元。当您发布单元后，单元的发布状态会显示为
`Published and Live`_ 或者 `Published Not Yet Released`_。

您可以从单元页面或者课程大纲中发布单元。

=======================================
从单元页面中能发布单元
=======================================

如下图所示，在单元状态面板中点击 **发布** 按钮：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-publish-button.png
 :alt: Unit status panel with Publish button circled


=======================================
从课程大纲中能发布单元
=======================================

如下图所示，在课程大纲中点击该单元旁边的发布按钮：

.. image:: ../../../shared/building_and_running_chapters/Images/outline-publish-icon-unit.png
 :alt: Publishing icon for a unit

.. note:: 
 只有对该单元做出修改后才会出现发布按钮。

.. _Discard Changes to a Unit:

****************************
放弃对单元的修改
****************************

当您编辑一个已发布单元时，修改的内容会自动保存在Studio中。
但是如果你不重新发布该单元，学生就无法看见修改后的单元内容。

如果您并不希望重新发布修改后的单元，在这种情况下，您可以放弃对单元的修改，这样Studio中的内容就会恢复到更改之前的版本。

只需点击状态面板中的 **放弃修改** 就可以让Studio中的内容恢复到更改之前的版本。

.. image:: ../../../shared/building_and_running_chapters/Images/unit-discard-changes.png
 :alt: Unit status panel with Discard Changes circled

.. caution::
“放弃修改”会永久地彻底删除更改内容。


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

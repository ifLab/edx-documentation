.. _Getting Started with Course Content Development:

###############################################
开始创建课程内容
###############################################

当您完成 :ref:`setting up your course<Setting up your Course Index>` 之后，
您可以开始创建课程内容。

本章简述建立课程内容过程中涉及的操作步骤，详情请点击以下链接：

* `Understanding Course Building Blocks`_
* `Creating New Course Content`_
* `Making Course Content Visible to Students`_
* `Revising Content`_

.. _Understanding Course Building Blocks:

************************************************
了解组成课程内容的要素
************************************************

在创建课程内容之前，您应该了解组成edX课程内容的要素。

* :ref:`The course outline<Developing Your Course Outline>` 是课程内容的容器，包括一个或多个章节。
* :ref:`Course sections<Developing Course Sections>` 是构成课程内容的重要组成部分，包括一个或多个小节。
* :ref:`Course subsections<Developing Course Subsections>` 是章节的组成部分，通常小节是按照主题或者其他规则划分的。一个小节中包括一个或者多个单元。
* 小节中的课程就是 :ref:`Course units <Developing Course Units>` ，单元是由一个或者多个组件组成的。
* :ref:`Course components<Developing Course Components>` 是单元中的内容，也是课程内容的组成部分。

.. _Creating New Course Content:

****************************************
创建新课程内容
****************************************

一旦您了解了edX课程的组成方式，您就可以开始组织您的课程内容，并将内容导入Studio。

在:ref:`course outline<Developing Your Course Outline>` 中创建 :ref:`sections<Create a Section>` 、:ref:`subsections<Create a
Subsection>` 和 :ref:`units<Create a Unit>` 。

您也可以通过:ref:`set the assignment type and due date<Set the Assignment Type and Due Date
for a Subsection>` 检测每一小节的学习效果。

在单元页面 :ref:`create components<Add a Component>` 。


另外，您也可以通过设置课程发布时间及发布单元来 :ref:`control content visibility<Controlling Content
Visibility>` 。

下图总结了创建课程内容的流程：

.. image:: ../../../shared/building_and_running_chapters/Images/workflow-create-content.png
 :alt: Diagram of the content creation process

我们建议您在创建的过程中 :ref:`test course content <Testing Your Course
Content>` 。

.. _Making Course Content Visible to Students:

******************************************************
确保课程内容对学生可见
******************************************************

在创建课程内容的同时，您还应该考虑何时将课程内容对学生开放。
课程内容的可见性取决于以下几点：

*  :ref:`course start date <Set Start and End Dates>`
*  :ref:`section<Set a Section Release Date>` 、
  :ref:`subsection<Set a Subsection Release Date>` 的发布日期
* 单元的 :ref:`publishing status<Hide a Unit from Students>` 
*  :ref:`Hide content from students<Hide a Unit from Students>` 设置
*  :ref:`Content Groups`
  
详细信息请见 :ref:`Controlling Content Visibility`.

.. _Making Course Content Searchable:

***********************************
Making Course Content Searchable
***********************************

Learners can search course text in :ref:`HTML components<Working with HTML
Components>` and video transcripts by using the **Search** box in the upper-left
corner of the **Courseware** tab. 

Before learners can search your course, Studio must index the content. Studio
indexes all new course content automatically when you :ref:`publish<Publish a
Unit>` the content. 

If necessary, you can manually reindex all of the content in your course at any
time. Typically, you would only manually reindex your course content if learners
see unexpected search results. To reindex your course content, select **Reindex
Content** in the upper-right corner of the **Course Outline** page. Reindexing
usually takes less than 30 seconds.

.. _Revising Content:

****************************
校正课程内容
****************************

您可以在任何时候校正课程内容。

* 如果章节、小节处于发布状态，那么您在调整 :ref:`reorganize sections, subsections, and units<Reorganize the
  Course Outline>` 时，学生可以立刻看见。

* When you :ref:`edit a unit<Edit a Unit>`, or :ref:`components<Add a
  Component>` within a unit, you must :ref:`publish<Publish a Unit>` those
  changes to make them visible to students.

The following diagram summarizes the content revision workflow and content
visibility:

.. image:: ../../../shared/building_and_running_chapters/Images/workflow-revise-content.png
 :alt: Diagram of the content creation process

It is recommended that you :ref:`test course content <Testing Your Course
Content>` during the revision process.

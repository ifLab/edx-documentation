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
*  :ref:`section<Set a Section Release Date>` 、 :ref:`subsection<Set a Subsection Release Date>` 的发布日期
* 单元的 :ref:`publishing status<Hide a Unit from Students>` 
*  :ref:`Hide content from students<Hide a Unit from Students>` 设置
*  :ref:`Content Groups`
  
详细信息请见 :ref:`Controlling Content Visibility`.

.. _Making Course Content Searchable:

***********************************
确保课程内容可搜索
***********************************

学生可以在 :ref:`HTML components<Working with HTML
Components>` 和视频脚本中通过 **课件** 栏左上角的 **搜索** 框搜索课程文本。

Studio必须为内容建立索引，学生才能搜索您的课程。当您 :ref:`publish<Publish a
Unit>` 时，Studio自动给所有新课程内容建立索引。

如果有必要，您随时可以手动重新建立索引。
一般情况下，您仅在学生看到不希望得到的搜索结果时重建课程内容索引。
在 **课程大纲** 页面的右上角选择 **为内容重建索引** 。重建过程只需要不到30秒。

.. _Revising Content:

****************************
校正课程内容
****************************

您可以在任何时候校正课程内容。

* 如果章节、小节处于发布状态，那么您在调整 :ref:`reorganize sections, subsections, and units<Reorganize the
  Course Outline>` 时，学生可以立刻看见。

* 在单元中 :ref:`edit a unit<Edit a Unit>` 或 :ref:`components<Add a
  Component>` 后，您必须重新 :ref:`publish<Publish a Unit>` ，这样学生才能看见新的内容。

下图总结了校正课程内容及控制内容可见性的流程

.. image:: ../../../shared/building_and_running_chapters/Images/workflow-revise-content.png
 :alt: Diagram of the content creation process

我们建议您在校正内容的同时 :ref:`test course content <Testing Your Course
Content>` 。

.. _Developing Your Course Outline:

###################################
创建课程大纲
###################################

您主要是在edX Studio的课程大纲中创建课程。本章主要概述课程大纲的操作方法。

* `Open the Course Outline`_
* `Example of a Developed Course in the Outline`_
* `View the Course Organization as a Student`_
* `Navigate the Course Outline`_
* `Add Content in the Course Outline`_
* `Modify Settings for Objects in the Course Outline`_
* `Publish Content from the Course Outline`_
* `Reorganize the Course Outline`_
* `Delete Content in the Course Outline`_
  
想了解如何在课程大纲中构建课程组成要素的相关信息请查看一下章节：

* :ref:`Developing Course Sections`
* :ref:`Developing Course Subsections`
* :ref:`Developing Course Units`
* :ref:`Developing Course Components`

****************************
打开课程大纲
****************************

浏览课程大纲：

#. 登录edX Studio。
#. 在 **我的课程** 页面选择想要创建的课程。

   当您打开一门课程时会默认打开课程大纲页面。

编辑课程时要打开课程大纲，首先点击内容菜单，选择 **大纲** 。
   
一门课程的课程大纲在首次预览时是没有任何内容的。

.. image:: ../../../shared/building_and_running_chapters/Images/outline_empty.png
 :alt: An empty course outline

您必须 :ref:`create the first section<Create a Section>`.
  
********************************************************
举例说明如何在课程大纲中搭建课程
********************************************************

下图介绍了课程大纲中一门课程的构成要素，包括章节、小节及单元。
当您创建好一门课程后，它就会显示成这个样子：

.. image:: ../../../shared/building_and_running_chapters/Images/outline-callouts.png
 :alt: An outline with callouts for sections, subsections, and units

如上图所示，这门课程包括以下三个部分：

#. :ref:`Sections<Developing Course Sections>`
#. :ref:`Subsections<Developing Course Subsections>`
#. :ref:`Units<Developing Course Units>`

:ref:`Components<Developing Course Components>` 不会显示在课程大纲中。但是，您可以通过点击包含这些组件的单元添加或者进入组件。
  
您可以查看上面的链接了解有关课程要素的信息。本章的剩余部分将阐述更多有关课程大纲的信息。

********************************************************
学生可见的课程安排
********************************************************

Studio课程大纲中显示的内容将直接呈现在学生学习管理系统中的课件库中。
下图展示了学生看到的课程内容形式：

.. image:: ../../../shared/building_and_running_chapters/Images/Course_Outline_LMS.png
 :alt: Image of course conent from student's point of view

.. _Navigating the Course Outline:

*******************************
管理课程大纲导航栏
*******************************

在studio中，您可以通过展开和收起章节、小节来管理课程大纲导航栏。
点击章节或者小节名称旁的下拉按钮展开，或者收起内容，如下图所示：

.. image:: ../../../shared/building_and_running_chapters/Images/outline-expand-collapse.png
 :alt: The outline with expand and collapse icons circled

扩展某一小节，那么这个小节中的所有单元都会呈现出来。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-with-units.png
 :alt: The outline with an expanded subsection

点击单元名称打开 :ref:`unit page<Developing Course Units>`.

.. _Add Content in the Course Outline:

************************************************
在课程大纲中添加内容
************************************************

您可以直接在大纲中添加章节、小节及单元。

点击大纲页面上方或者下方的 **新建章节** 按钮新建章节。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-create-section.png
 :alt: The outline with the New Section buttons circled

在章节后面添加小节，先扩展该章，然后点击 **新建小节** 按钮。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-new-subsection.png
 :alt: The outline with the New Subsection button circled

在小节后面添加单元，先扩展该小节，然后点击 **新建单元** 按钮。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-new-unit.png
 :alt: The outline with the New Subsection button circled

打开 :ref:`unit<Developing Course Units>` 页面。


.. the following note is for prerequisite exams, which are currently released in open edx only and not on edx.org.  when they are available on edx.org, this note should no longer be conditionalized.

.. only:: Open_edX

    .. note::
      If you want to require an entrance exam for your course, you also create
      the exam in the course outline. Before you can create an exam, you must
      set your course to require an entrance exam in Studio. For more
      information, see :ref:`Require an Entrance Exam`.

.. _Modify Settings for Objects in the Course Outline:

***************************************************
在课程大纲中更改内容设置
***************************************************

您可以在课程大纲中更改章节、小节及单元的设置，包括：

* :ref:`Set a Section Release Date`
* :ref:`Hide a Section from Students`
* :ref:`Set a Subsection Release Date`
* :ref:`Set the Assignment Type and Due Date for a Subsection`
* :ref:`Hide a Subsection from Students`
* :ref:`Hide a Unit from Students`

点击“设置”按钮更改更改章节、小节及单元的设置。如下图圆圈标记所示：

.. image:: ../../../shared/building_and_running_chapters/Images/settings-icons.png
 :alt: Settings icons in the course outline

详细信息请点击上文中的链接。


.. _Publish Content from the Course Outline:

************************************************
在课程大纲中发布内容
************************************************

您可以发布整个章节、小节中的新单元或者修改后的单元，也可以单独发布单元。

点击章节、小节中的“发布”按钮发布新单元或者修改后的单元内容。如下图圆圈标记所示：

.. image:: ../../../shared/building_and_running_chapters/Images/outline-publish-icons.png
 :alt: Publishing icons in the course outline

.. note:: 
 只有在课程内容发生改变时“发布”按钮才会显现。

详细信息请参见以下内容：

* :ref:`Unit Publishing Status`
* :ref:`Publish all Units in a Section`
* :ref:`Publish all Units in a Subsection`
* :ref:`Publish a Unit`


.. _Reorganize the Course Outline:

************************************************
重新整理课程大纲
************************************************

在大纲页面中，您可以通过移动章节、小节及单元的位置重组课程大纲。

要移动某个元素时，只需将鼠标悬停在屏幕右侧的元素句柄上直至鼠标指针变成四方向箭头，如下图所示：已选中“第一课——入门指南”：

.. image:: ../../../shared/building_and_running_chapters/Images/outline-drag-select.png
 :alt: A subsection handle selected to drag it

然后，将鼠标选中并拖动需要移动的部分。

如果您扩展了目标章节，那么，当你在移动大纲中的某一要素时，会出现一条蓝色的直线告知您松开鼠标后该要素会出现在的地方。
如下图所示，“第一课——入门指南”会移至到“介绍”后。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-drag-new-location.png
 :alt: A subsection being dragged to a new section 	

如果您没有扩展目标章节，那么移动要素至有效的位置时，目标章节会出现蓝色的边框，这时您可以松开鼠标。
如下图所示，“第一课——入门指南”会移至到收起的章节“介绍”后。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-drag-new-location-collapsed.png
 :alt: A subsection being dragged to a new section 

.. _Delete Content in the Course Outline:

************************************************
在课程大纲中删除内容
************************************************

您可以在课程大纲中删除章节、小节及单元。

.. warning::  
 删除的内容无法恢复。为避免删除有用到的内容，我们建议您将目前不需要的内容移到某一章节中然后设置成不发布的状态。

点击“删除”按钮删除不需要的内容。

.. image:: ../../../shared/building_and_running_chapters/Images/outline-delete.png
 :alt: The outline with Delete icons circled

之后会弹出对话框让您确认删除。

.. note::
 确认“删除”将删掉该要素中包含的所有内容。例如，您删除某一小节的内容，那么该小节中的所有单元也会随之删除。

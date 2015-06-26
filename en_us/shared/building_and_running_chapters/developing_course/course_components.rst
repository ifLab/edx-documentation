.. _Developing Course Components:

###################################
创建课程组件
###################################

本章主要描述如何创建课程组件：

* `What is a Component`_
* `Add a Component`_
* `Edit a Component`_
* `Duplicate a Component`_
* `Delete a Component`_
* `Components that Contain Other Components`_

要了解更多有关特殊组件类型的信息，请参考以下章节内容：

* :ref:`Creating Course Content Index`
* :ref:`Exercises and Tools Index`

.. _What is a Component:

********************
什么是组件
********************

课程组件是单元的组成部分，包括了您最具体的课程内容。一个单元可能包含一个或多个课程组件。

学生能看见某个单元下所有元素的名称，只需将鼠标停留在课程进度条的某个单元上即可。

.. image:: ../../../shared/building_and_running_chapters/Images/ComponentNames_CourseRibbon.png
 :alt: Image of the component list for a unit

系统默认的课程组件有以下四种：

* **讨论组件** 该组件在为您的课程提供讨论空间，以便学生就某节课交换意见。
* **HTML组件** 该组件是您能够给课程添加文本、图像以及其他不同类型的学习工具。该板块中的内容默认为HTML格式。
* **问答组件** 该组件方便您布置各种练习题或进行课堂提问，从简单的单项选择，到复杂的电路原理图的练习均可。
* **视频组件** 该组件包括您在课程中要播放的视频。

.. _Add a Component:

********************
添加组件
********************

在 **添加新组件** 选项下单击您想添加的组件类型以添加组件。

.. image:: ../../../shared/building_and_running_chapters/Images/AddNewComponent.png
  :alt: Image of adding a new component

更多信息请参考相应组件的软件文档：

- :ref:`Working with Discussion Components`
- :ref:`Working with HTML Components`
- :ref:`Working with Problem Components`
- :ref:`Working with Video Components`
  
添加组件以后，您必须
:ref:`publish the unit<Publish a Unit>` ，学生才能看到。

.. _Edit a Component:

********************
编辑组件
********************

点击 **编辑** 以编辑组件。

.. image:: ../../../shared/building_and_running_chapters/Images/unit-edit.png
  :alt: Image of a unit with Edit icon circled

按照指导编辑组件。

编辑组件之后，您需要
:ref:`publish the unit<Publish a Unit>` 让学生看到组件。

=====================================
设置组件的显示名
=====================================

所有组件都有显示名，当编辑组件时，显示名会出现在标题栏。
当学生将鼠标指针停留在某个单元标记上时，也能看见组件的显示名。

如何设置组件的显示名：

#. 编辑组件
#. 单击 **设置**
#. 在 **显示名** 一栏输入名称内容

  .. image:: ../../../shared/building_and_running_chapters/Images/display-name.png
   :alt: Image of the Display Name field for a component.

4. 单击 **保存**

不同的板块类型在“设置”对话框中的字段不同，但都有 **显示名** 字段。

.. _Duplicate a Component:

**********************
复制组件
**********************

当复制某个板块时，该组件的正下方会出现一个新拷贝，您可对它进行操作。
通常而言，复制组件然后编辑拷贝能更快地创建新内容。

单击组件标题栏中的“复制”图标：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-dup.png
  :alt: Image of a unit with Duplicate icon circled

按照提示编辑您的组件。

复制组件之后，您需要重新 :ref:`publish the unit<Publish a Unit>` ，学生才能看到新的组件。

.. note::  您不能复制内容实验。

.. _Delete a Component:

**********************
删除组件
**********************

.. caution:: 
 删除组件前请再次确认是否真的需要删除。删除操作是不可逆的。

遵循以下步骤删除组件：

#. 点击标题旁边的删除按钮：

.. image:: ../../../shared/building_and_running_chapters/Images/unit-delete.png
  :alt: Image of a unit with Delete icon circled

2. 当确认框弹出时，点击 **是的，删除这个组件** 。

组件删除后，您需要重新 :ref:`publish the unit<Publish a Unit>` ，否则学生仍能看到已删除的组件。

.. _Components that Contain Other Components:

******************************************
组件嵌套
******************************************

在特定情况下，您可能会设置组件中嵌套另一个组件。
例如，如果您希望组件中包含条件组件或内容实验，您必须在创建嵌套组件。
详情请参考
:ref:`Creating Content Experiments` for more information.

包含其他组件的组件称为 **父组件**；被包含的组件称为 **子组件** 。

在单元页中，父组件显示组件名和 **查看** 链接，如下：

.. image:: ../../../shared/building_and_running_chapters/Images/component_container.png
 :alt: Image of a unit page with a parent component


==================================================
编辑父组件
==================================================

父组件不直接包含内容。HTML文件、视频和程序都包含在子组件中。

父组件显示组件名。当单元为草稿或属性为私有时，点击父组件中的 **编辑** 项更改组件名。

.. note:: 
  特殊类型的父组件，如内容实验，可以编辑附加属性。
  


======================================
查看子组件
======================================

当您在父组件中点击 **查看** 时，父组件页面开启，页面中显示所有的子组件。
下图中子组件含有HTML组件和视频文件：

.. image:: ../../../shared/building_and_running_chapters/Images/child-components-a.png
 :alt: Image of an expanded child component

单击子组件名旁边的箭头可以收起组件内容：

.. image:: ../../../shared/building_and_running_chapters/Images/child-components.png
 :alt: Image of a child component page

再次点击箭头可以展开内容：

详情请参阅：

* `Edit a Component`_
* `Set the Display Name for a Component`_
* `Duplicate a Component`_
* `Delete a Component`_

======================================
添加子组件
======================================

如果组件内含的单元为私有属性或草稿，您可以为此组件添加子组件。

打开父组件页面，在 **添加新组件** 栏中选择您想添加的子组件类型。

.. image:: ../../../shared/building_and_running_chapters/Images/AddNewComponent.png
  :alt: Image of adding a new component

更多信息请查阅：

- :ref:`Working with Discussion Components`
- :ref:`Working with HTML Components`
- :ref:`Working with Problem Components`
- :ref:`Working with Video Components`


======================================
组件中的XML文件
======================================

如果您用XML创建组件，您可以将XML课程导入Studio中以确认其结构是否符合您的要求。

更多关于使用XML文件的信息，包括关于术语的信息，请参阅 `edX XML Tutorial <http://edx.readthedoc
s.org/projects/devdata/en/latest/course_data_formats/course_xml.html>`_ 。

下图是Studio中用来创建单元和组件的XML。

单元的XML是：

.. code-block:: xml

    <vertical display_name="Unit 1">
        <html url_name="6a5cf0ea41a54b209e0815147896d1b2"/>
        <vertical url_name="131a499ddaa3474194c1aa2eced34455"/>
    </vertical>

上例中的 ``<vertical url_name="131a499ddaa3474194c1aa2eced34455"/>`` 元素引用自父组件。
 
.. code-block:: xml

    <vertical display_name="Parent Component">
        <vertical url_name="2758bbc495dd40d59050da15b40bd9a5"/>
        <vertical url_name="c5c8b27c2c5546e784432f3b2b6cf2ea"/>
    </vertical>

两个引用自父组件的vertical包含了您课程中的实际内容。

.. code-block:: xml

    <vertical display_name="Child Component A">
        <html url_name="4471618afafb45bfb86cbe511973e225"/>
        <video url_name="fbd800d0bdbd4cb69ac70c47c9f699e1"/>
    </vertical>

.. code-block:: xml

    <vertical display_name="Child Component B">
        <html url_name="dd6ef295fda74a639842e1a49c66b2c7"/>
        <problem url_name="b40ecbe4ed1b4280ae93e2a158edae6f"/>
    </vertical>

理论上，组件嵌套的层数是无限的。

======================================
学生视角查看嵌套组件 
======================================

在学生视角中，所有父组件和子组件都陈列在单元页面中。
下图是学生视角中的单元界面：

.. image:: ../../../shared/building_and_running_chapters/Images/nested_components_student_view.png
 :alt: Image of the student's view of nested components

.. note:: 
 嵌套组件的可见性取决于所在单元的可见性。父单元必须是对学生公开的属性，学生才能看到嵌套组件。
 更多信息请参阅： :ref:`Unit States and Visibility to Students`.


*******************************
Reorganizing Child Components 
*******************************

You can reorganize child components through the same drag and drop process you
use for other objects in your course outline. You hover over the element handle
on the right side of the screen until the mouse pointer changes to a four-
headed arrow. Then, click and drag the element to the location that you want.

Furthermore, when you have multiple levels of nesting, you can drag a child
component into a different parent component, if both parents are expanded. For
example, you can select the video component that is in Child Component A and
drag it into Child Component B. Select the video component, and as you drag it
into Child Component B, release the mouse button when a dashed outline of the
component you are moving appears in the new location:

.. image:: ../../../shared/building_and_running_chapters/Images/drag_child_component.png
 :alt: Image of dragging a child component to a new location

You can also drag a child component outside of a parent, so that the child
moves to the same level as the parent.

.. note:: 
  For content experiments, you cannot drag a child component outside of a test
  group.

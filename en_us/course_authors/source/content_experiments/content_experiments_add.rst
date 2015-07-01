.. _Add Content Experiments to Your Course:

#########################################
为您的课程添加内容实验
#########################################

在您 :ref:`enable content experiments <Enable Content Experiments>` 以及
:ref:`set up group configurations in Studio <Set up Group Configurations in edX
Studio>` 之后，您可以为您的课程添加内容实验，请参阅：

* :ref:`Add a Content Experiment in Studio`
* :ref:`Add a Content Experiment in OLX`

.. _Add a Content Experiment in Studio:

********************************************
在Studio添加内容实验
********************************************

您可以在单元页面或容器页面中添加内容实验。
在Studio中，您可以创建并查看某个容器页面中所有学习组的实验内容。
请参阅  `Create Content for Groups in the Content
Experiment`_ 。

当学生查看带有内容实验的课程单元时，不会察觉到正在进行的内容实验。
她看不见实验名称，只能看见您给他所在的实验小组分配的内容。
对于学生而言，带有内容实验的课程单元与其他课程单元无异。

在Studio中配置内容实验，您需要：

#. `Create the content experiment`_.
#. `Create content for groups in the content experiment`_.
   
成功创建内容实验后，您可以更改分组模式。
详情请参阅 `Change the Group Configuration for a Content Experiment`_ 。

===============================
创建内容实验
===============================

#. 您需要在单元页面中的 **添加新组件** 目录下点击 **高级** 。

#. 选择 **内容实验** 。
   
   新的内容实验已经添加到此单元中：

   .. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_block.png
    :width: 800
    :alt: The content experiment component in a unit page

   对该模块的操作与其他课程模块无异。详情请参考 :ref:`Developing Course Components` 页面。

#. 单击 **选择分组模式** 或 **编辑** 均可打开内容实验模块。

   .. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_editor.png
    :alt: The content experiment editor

#. 在 **分组模式** 旁边的的下拉选项中，选择一个分组模式。

#. 在 **显示名** 字段下，键入本模块在Studio中显示的名称。该名称只在Studio中可见，对学生端不可见。

#. 单击 **保存** 。

内容实验显示为一个大模块，其中包含了许多其他小模块。更多信息请参见
:ref:`Components that Contain Other Components` 章节中的内容。

.. note::  内容实验模块无法复制。

现在，您可以为实验小组添加实验内容了。

=====================================================
为实验小组添加实验内容
=====================================================
   
在内容实验模块中选择一个分组模式，单击 **查看** 。

自动弹出的内容实验页面包含了一个容器页面，该页面下又涵盖了您选择的分组模式以及该模式中的所有实验组。
例如，您选择的分组模式包含A组和B组，则您会看见如下页面：

.. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_container.png
 :alt: The content experiment page with two groups

您可以给这两个小组选择添加实验内容，具体操作方法与其他容器页面相同。
更多信息请参见 :ref:`Components that Contain Other Components` 章节中的内容。

例如，您可以给A组添加一个HTML模块或视频模块：

.. image:: ../../../shared/building_and_running_chapters/Images/a_b_test_child_expanded.png
 :alt: Image of an expanded A/B test component

.. note:: 
  有时候，预留一个没有内容的空组对于实验来说非常有用。
  比如，如果一个小组正在看视频，另一个小组没有内容，您就可以根据学生表现来分析视频的效果。


========================================================
为实现内容实验更改分组模式
========================================================

您可以根据某个内容实验的需求更改分组模式。当分组模式更改后，您需要给新创建的小组添加模块或组件。
您可以沿用原来的模块，也可以创建新模块。

.. warning::
  如果某个实验对学生可见，更改该实验的分组模式会影响实验数据。

如何改变分组模式：

#. 打开该内容实验的单元页面。

#. 在内容实验模块中，单击 **编辑** 。

   .. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_editor_group2.png
    :alt: The content experiment editor with a group configuration selected

#. 选择您需要的分组模式。

#. 单击 **保存** 。

#. 现在您需要为新创建的实验组添加模块或组件。单击 **查看** 打开内容实验页面。

   您会发现，新创建的分组模式下空空如也，您在之前的分组模式中添加的模块和组件都被转移到了 **非活动组** 区域中。

   .. image:: ../../../shared/building_and_running_chapters/Images/inactive_groups.png
    :alt: Components in inactive groups

#. 您可以将 **非活动组** 中的内容拖拽到新分组中，也可以在新分组中创建新的内容。

.. import OLX-content experiment doc that's shared in OLX guide.

.. include:: ../../../shared/subsections/content_experiments/content_experiments_OLX.rst

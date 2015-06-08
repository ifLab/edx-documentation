.. _Configure Your Course for Content Experiments:

#####################################################
配置带有内容实验的课程
#####################################################

本章将描述如何配置一堂带有内容实验的课程。以下是章节一览：

* :ref:`Enable Content Experiments`
* :ref:`Overview of Group Configurations`
* :ref:`Set up Group Configurations in edX Studio`
* :ref:`Guidelines for Modifying Group Configurations`
* :ref:`Set Up Group Configuration for OLX Courses`

.. _Enable Content Experiments:

****************************************
启用内容实验
****************************************

想要启用内容实验，您需要在高级设置中的 **高级模块列表** 下添加 ``split_test`` 。

.. note::  
  ``split_test`` 即“内容实验”在edX平台中的内部名称。

#. 在 **设置** 菜单中，选择 **高级设置** 。

#. 在 **高级设置** 页面中，选择 **高级模块列表** 。

#. 在 **高级模块列表** 字段下，添加 ``"split_test"``。注意，包括双引号。

   如果您需要输入多个值，值与值之间请用逗号分隔
   (``,``)。

   例如，在 **高级模块列表** 字段中的文字内容如下：

   .. code-block:: json
     
     [
       "lti",
       "word_cloud",
       "split_test"
     ]

#. 在页面底部，单击 **保存更改** 。

.. _Overview of Group Configurations:

****************************************
分组模式概述
****************************************

在创建内容实验之前，您需要为您的课程指定至少一种分组模式。

分组模式决定了某项内容实验中学生组的数量。您在课程中可以配置任意数量的分组。
当创建内容实验时，您可以选择需要使用的分组模式。

例如，您可以在课堂上安排两组不同时段的内容实验，其中一项的实验内容是看一段视频或完成一项阅读任务。
您可以在实验中就某一问题提出探讨，以确定哪一组对实验材料掌握得更透彻。
在这个实验中，您应该将学生分为两个组。

而在另一个实验中，您可能需要就同一探讨主题以四种不同方式提问，这种情况下，就应该将学生配置为四个学习组。

=======================================
将学生分配到学习组
=======================================

edX 平台通过分组模式将学生分成不同学习组。

分组方式有如下几种：

* 动态分组法

  当某个学生第一次查看带有分组模式的内容实验时，edX 平台会将该学生分到某个小组中。

* 随机分组法
  
  系统随机将某个学生随机分到某个小组里。
  
* 平均分配法
  
  edX平台会随时跟踪每个组的规模，平均地将新学生分配到每个组中。
  例如，如果您的一个分组模式中有两个学习组，每个小组将包含该课程学生总数的50%；
  如果分组模式中有四个学习组，每个小组将包含该课程学生总数的25%。

* 永久分配法
  
  无论您设立了多少组分组模式相同的内容实验，学生的分组都固定不变。


.. _Set up Group Configurations in edX Studio:

************************************************
在edX Studio中设置分组模式 
************************************************

.. note:: 
  您需要先 :ref:`enable content experiments<Enable Content Experiments>` 才能进行本项工作。

要设置分组模式，在 **设置** 菜单下选择 **分组模式** ，打开 **分组模式** 页面。

在该页面中您可以:ref:`create<Create a Group Configuration>`,
:ref:`edit<Edit a Group Configuration>` ，以及 :ref:`delete<Delete a Group
Configuration>` 分组模式。您也可以 :ref:`view experiments that
use a group configuration<View Experiments that Use a Group Configuration>` 。

.. _Create a Group Configuration:

=============================
创建分组模式
=============================

您可随时创建想要的分组模式。

#. 在 **分组模式** 页面，在 **学习组** 下，单击
   **新的学习组** 按钮打开下面的页面：

  .. image:: ../../../shared/building_and_running_chapters/Images/create-group-config.png
   :width: 800
   :alt: Create a New Group Configuration page

2. 在 **分组模式名称** 中输入名称。 请使用符合意义的名称，因为您将在创建内容实验中选择分组模式。
学生页面将不会显示分组模式名称。

#. 根据需要为模式名称添加描述。
   
#. 新的模式将默认含有两个小组。根据需要更改、添加或删除模式下的小组。
   每个模式中必须含有至少一个小组。

  * 根据需要更改模式名称。 您可以在Studio单元页中看到小组名称，
    小组名称对学生不可见。       
  * 点击 **添加一个小组** 来为当前模式添加一个新的小组。
    
  * 点击现有小组右边的 **X** 按钮可将该小组从模式中删除。
    每个模式中必须含有至少一个小组。

5. 点击 **创建** 可添加一个新的模式。
   
完成创建后，新的分组模式就会出现在页面列表中。您可以看见该模式下包含的小组数量，
以及该分组模式在课堂上的使用状况。

.. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_one_listed.png
 :width: 800
 :alt: The Group Configurations page with one group configuration


  
.. _Edit a Group Configuration:

=============================
编辑分组模式
=============================

.. important:: 您可随时更改分组模式的名称。但是，如果您想更改该模式的其他元素，
   尤其是正在课堂上使用的分组模式，请先参考 `Guidelines for Modifying Group Configurations` 。

#. 在 **分组模式** 页面中， 将鼠标悬停在某个模式上，
   单击 **编辑** 。
   
   .. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_edit.png
    :alt: The Group Configurations page with Edit button

   打开如下页面：

   .. image:: ../../../shared/building_and_running_chapters/Images/save-group-config.png
    :alt: Edit a Group Configuration page

#. 根据需要更改模式名称或描述。

#. 根据需要更改模式下的小组。 详情参考：:ref: `Create a Group
   Configuration`_ 。
   
#. 单击 **保存** 保存更改。

.. _Delete a Group Configuration:

=============================
删除分组模式
=============================

.. note:: 
 您无法删除目前正在内容实验中使用的分组模式。

#. 在 **分组模式** 页面中，将鼠标悬停在某个分组模式上，单击
   删除图标。

  .. image:: ../../../shared/building_and_running_chapters/Images/group-configuration-delete.png
   :alt: Edit a Group Configuration page

2. 在跳出的删除确认框中，单击 **删除**.


.. _View Experiments that Use a Group Configuration:

===============================================
查看分组模式在内容实验中的使用状况
===============================================

当使用分组模式时，您可以查看正在使用某个模式的内容实验。

在 **分组模式** page, 页面中，单击某个分组可以查看该组的详细信息。
您可在页面中看见一个链接，指向正在使用该模式的内容实验：

.. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_experiments.png
 :alt: A group configuration with the experiments using it circled

单击某个链接转到包含该内容实验的单元页面。


===============================================
在实验中查看分组模式
===============================================

当您在进行内容实验时，您可以使用以下两种方式查看该实验使用的分组模式详情：

* 在包含该实验的单元页面中，单击分组模式的名称即可。

.. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_group_config_link.png
 :alt: Content experiment in the unit page with the group configuration link
     circled

* 或者，在内容实验页面顶部，单击分组模式名称。

.. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_page_group_config_link.png
 :alt: Content experiment page with the group configuration link circled

上述两种方法都可以打开该分组模式：

.. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_experiments.png
 :alt: A Group Configuration with the experiments using it circled

您可以使用分组模式页面中的链接回到对应的内容实验页面。

.. import OLX-content experiment doc that's shared in OLX guide.

.. include:: ../../../shared/subsections/content_experiments/content_experiments_group_modify_guidelines.rst

.. include:: ../../../shared/subsections/content_experiments/content_experiments_policies.rst

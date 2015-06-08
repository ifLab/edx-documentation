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

2. Enter a name in the **Group Configuration Name** field. Use a meaningful
name, because you will select from group configuration names when you create
content experiments. Students do not see the group configuration name.

#. Optionally, enter a description for the new group configuration.
   
#. By default, a new configuration already contains two groups. Modify the
   groups or add and delete groups as needed. A group configuration must have at
   least one group.

  * Modify group names as needed. You see group names in the unit page in
    Studio, but group names are not visible to students.       
  * Click **Add another group** to include another group as part of
    the configuration. 
  * Click the **X** to the right of an existing group to remove it from the
    configuration. A group configuration must have at least one group.

5. Click **Create** to save the new group configuration.
   
The group configuration is then listed in the page. You can see the number of
groups that the configuration contains, as well as whether the configuration is
in use in the course:

.. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_one_listed.png
 :width: 800
 :alt: The Group Configurations page with one group configuration


  
.. _Edit a Group Configuration:

=============================
Edit a Group Configuration
=============================

.. important:: You can change the name of a group configuration at any time.
   However, before you modify any other characteristics of a group configuration
   that is currently used in a running course, review `Guidelines for Modifying
   Group Configurations`_.

#. On the **Group Configurations** page, hover over the group configuration and
   click **Edit**.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_edit.png
    :alt: The Group Configurations page with Edit button

   The following page opens:

   .. image:: ../../../shared/building_and_running_chapters/Images/save-group-config.png
    :alt: Edit a Group Configuration page

#. Modify the name and description as needed.

#. Modify groups in the configuration as needed. See `Create a Group
   Configuration`_ for details.
   
#. Click **Save** to save your changes.

.. _Delete a Group Configuration:

=============================
Delete a Group Configuration
=============================

.. note:: 
 You can only delete a group configuration that is not currently used in a
 content experiment. You cannot delete a group configuration that is used in a
 content experiment.

#. On the **Group Configurations** page, hover over the group configuration and
   click the Delete icon. 

  .. image:: ../../../shared/building_and_running_chapters/Images/group-configuration-delete.png
   :alt: Edit a Group Configuration page

2. When prompted to confirm the deletion, click **Delete**.


.. _View Experiments that Use a Group Configuration:

===============================================
View Experiments that Use a Group Configuration
===============================================

You can view the experiments that use each of your group configurations.

On the **Group Configurations** page, click the name of a group to see its
details. You see links to experiments that use the group configuration:

.. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_experiments.png
 :alt: A group configuration with the experiments using it circled

Click a link to go to the unit page that contains the experiment.


===============================================
View a Group Configuration from an Experiment
===============================================

When working with a content experiment, you can view details about the group
configuration used by that experiment in two ways:

* In a unit that contains a content experiment, in the content experiment block,
  click the name of the group configuration.

.. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_group_config_link.png
 :alt: Content experiment in the unit page with the group configuration link
     circled

* At the top of the content experiment page, click the name of the group
  configuration.

.. image:: ../../../shared/building_and_running_chapters/Images/content_experiment_page_group_config_link.png
 :alt: Content experiment page with the group configuration link circled

In both cases, the group configuration opens:

.. image:: ../../../shared/building_and_running_chapters/Images/group_configurations_experiments.png
 :alt: A Group Configuration with the experiments using it circled

You can use the link in the group configuration to return to the unit that
contains the content experiment.

.. import OLX-content experiment doc that's shared in OLX guide.

.. include:: ../../../shared/subsections/content_experiments/content_experiments_group_modify_guidelines.rst

.. include:: ../../../shared/subsections/content_experiments/content_experiments_policies.rst

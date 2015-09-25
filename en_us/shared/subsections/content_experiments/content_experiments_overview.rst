.. _内容实验概述:

#################################
内容实验概述
#################################

你可以使用内容实验展示不同的课程内容不同的学生小组. 也被称为“A/B测试”或"对比测试",内容实验允许你研究和比较不同组的学生的表现来了解你的课程内容的相对有效性。

关于内容实验的分析信息都在`edX Researcher Guide`_中.

.. _edX Researcher Guide: http://edx.readthedocs.org/projects/devdata/en/latest/internal_data_formats/tracking_logs.html#a-b-testing-events

更多信息, 请看:

* :ref:`Configure Your Course for Content Experiments`
* :ref:`Add Content Experiments to Your Course`
* :ref:`Test Content Experiments`

.. _Courses with Multiple Content Experiments:

******************************************
带有多个内容实验的课程
******************************************

你可以在你的课程中创建创建多个内容实验. 你可以设置每个内容实验都使用相同的学生小组，你也可以为每个实验设置不同的小组.

.. important::

  如果你的课程有多个内容实验,你提前决定是否实验都使用相同的学生小组或者每个实验设置不同的小组是十分关键的。如果两个实验使用同一个小组,那么任何在A组第一个实验的学生也将在A组第二个实验。如果你想要实验更加自主, 那么这个就必须使用不同的小组了以便学生随机分配到每个实验中.

要决定学生可用的分组, 你需要设置小组配置:ref:`使用Studio <在edX Studio设置学生团队配置>`或者:ref:`使用XML <对OLX课程设置小组配置>`.

你然后可以选择团队设置使用何时添加文本实验、:ref:`使用Studio <在edX Studio设置学生团队配置>` or
:ref:`使用XML <对OLX课程设置小组配置>`.

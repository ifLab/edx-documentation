.. _Cohorts Overview:


#############################
使用队列功能建立课程群
#############################

If you want to create smaller communities in your course, or design different
course experiences for different groups of students, you can :ref:`set up
cohorts<Enabling and Configuring Cohorts>` in your course.  In discussion topics
that are divided by cohort, students can also communicate and share experiences
privately within the cohort that they are assigned to. Cohort-specific
discussion opportunities can help students develop a sense of community, provide
specialized experiences, and encourage deeper, more meaningful course
involvement.

If you use cohorts in your course, you define a set of cohorts that reflect
communities of students, then select a strategy for :ref:`assigning students to
cohorts<Options for Assigning Students to Cohorts>`.

.. note::    
   * 每个学生都必须分配到队列中。这样每个学生都能阅读所有讨论课题，并就课题贡献自己的力量。


   * 每个学生只能分配到一个队列中。

   为保证持续的课堂体验，课程开始后，不应变更学生的分队模式。

更多信息请看以下两节的内容：

* :ref:`Enabling and Configuring Cohorts`

* :ref:`Setting Up Discussions in Courses with Cohorts<Set up Discussions in
  Cohorted Courses>`

* :ref:`Moderating Discussions for Cohorts`

关于“课题讨论”的更多信息请参考 :ref:`Discussions`.


.. _Options for Assigning Students to Cohorts:

*****************************************
课题讨论选项
*****************************************

Students are assigned to cohorts either automatically or manually, depending on
the types of cohort that you create in your course. Manual cohorts do not have
students assigned to them unless you manually add students. Automatic cohorts
have students randomly assigned to them if students do not belong to any cohort
by the time they access the course content (including the course **Discussion**
page or content-specific discussion topics). If you have not created any
automated cohorts by the time students access course content, a default
automated cohort is created and used for automatic assignment, so that no
student in the course is without a cohort.

Determine the basic strategy that you will use to create cohorts for your
course. An automated assignment strategy means that you create cohorts to which
students are assigned automatically and randomly. A manual assignment strategy
means that you create cohorts to which students are assigned only when you or
your course team manually adds them. You can use a hybrid assignment method by
creating a combination of automated and manual cohorts. Typically, your purpose
in including the cohort feature in your course determines which assignment
option you use for your course.

.. note:: You can add students manually to any cohort, whether it was created as
   an automated cohort or a manual cohort.

.. note:: Although you can change the assignment method of a cohort at any time
   after you create it, you should have a cohort assignment strategy in mind as
   you design your course, and only make changes to cohorts while the course is
   running if absolutely necessary. Be aware of the implications of changing
   cohort configuration while your course is running. For more information, see
   :ref:`Altering Cohort Configuration`. In general, to provide students with a
   consistent experience throughout the course run, do not change cohort
   configuration or a student's cohort assignment after your course begins.

For more information about strategies for assigning students to cohorts, see the
following topics.

* :ref:`All Automated Assignment`

* :ref:`All Manual Assignment`

* :ref:`Hybrid Assignment`

* :ref:`Default Cohort Group`
  


.. _All Automated Assignment:

========================================================
自动分队：让大规模的讨论更易管理
========================================================

在一些规模较大的课程中，关于某个讨论课题的帖子数量可谓堆积成山，
令人望而却步。对这类课程而言，将课程参与者分为几个小队可以有效管理发帖、
回帖以及评论数量，同时更有助于培养群体意识。

采用这种分队策略，您需要启用分队功能，并创建一组“自动”分队。
创建成功后，当一个学生第一次查看“课程讨论”页面，或其他特殊讨论课题时，
将被自动随机分配到某个小组中。所有被分到同一小组的学生组成一个队列。

这几条操作指南基于本平台对大规模在线开放课程团队的管理经验，
能够帮助您在课程中正确决定自动分队队列的数量。

* 每个队列的规模不应太小，否则将很难调动学生的积极性，也很难从多方面角度收集意见；
  同时也不应太大，否则容易使团队一盘散沙，丧失集体意识。
  随机分组下的队列规模应在200至500人之间为宜。

* 每10000名学生中，能从头到尾保持讨论积极性的约为200至400人左右。

* 将预计的课程参与人数除以10000。

* 得到的结果即为自动分队队列的数量。

比如，一项课程开始两天前，报名学生人数为80000人。
课程团队启用分队功能，创建了8个自动分队队列。
当学生访问讨论页面并查看讨论模块时，会被随机分配到一个队列中。
在分队讨论课题中，学生只能阅读、回复同一小队成员发布的内容。

更多信息请参考 :ref:`Implementing the Automated Assignment
Strategy`.


.. _All Manual Assignment:

=====================================================
手动分组：“人以群分”
=====================================================

在SPOC（小型私人在线课程）以及其他中小规模的课堂中，
教师可以根据学生的已知共性创建队列。比如，您的学生可能来自不同的公司，
可能拥有不同教育背景，参加了不同的团体等等。将学生按照不同共性分组，
学生能够私下讨论自己感兴趣的话题，从而寻找符合特定团体利益的资源和创意。

在使用这种分组策略之前，您需要事先了解您的学生在现实生活中属于哪一类群体。
您可以启用分队模式，并将默认设置修改为“手动”（manual）分组，
然后您可以将学生一一分配到这些手动分队队列中。
无论课程开始前后，所有加入课程的学生都必须至少被分配到一个队列中。

.. note:: 保证每个学生都有组可分，您可以在手动分队队列之外再创建一个单独的自动分队队列。
   这部分内容会在下一节中提到。如果您没时间创建队列，系统会自动创建一个默认分队以保证所有学生都有组可分。

更多信息请参考 :ref:`Implementing the Manual Assignment Strategy`.


.. _Hybrid Assignment:

=============================================================
Hybrid Assignment: Accommodating Small Groups Within a Course
=============================================================

For some courses, the manual assignment strategy is not feasible to execute, and
the automated assignment strategy does not accommodate existing cohorts in the
student body. The enrollment might be too large to complete manual assignments
effectively, or only some of the students might have strong defining
characteristics among an otherwise diverse student body. For these courses, you
can use a hybrid of the two strategies to implement cohorts.

An example is a course that enrolls members of an alumni association. The alumni
want an opportunity to have private interactions, so manual assignment of those
students to a cohort makes sense. For other students in the class, manual
assignment is not needed: you can create one or more automated cohorts for the
remaining learners in the course.

Before you implement the hybrid strategy, you identify the characteristics that
define existing cohorts in the student body. You also decide whether you want
the remaining students in the course to be divided into their own, similarly-
sized cohorts, or if you want them all to be in just one other cohort.

After you enable cohorts, you create a manual cohort for each student group that
you identified. You manually assign students who belong to each group to the
corresponding cohort. You also set up automated cohorts for the other students
in the course, or rely on the default automated cohort. Any students who are not
assigned to a manual cohort are automatically assigned to one of the automated
cohorts or to the default cohort when they first view any course content,
including the course **Discussion** page or content-specific discussion topics.
For best results when you use this strategy, you should complete all manual
cohort assignments before the course starts and before students begin viewing
course content and discussion topics.

For more information, see :ref:`Implementing the Automated Assignment
Strategy` and :ref:`Implementing the Manual Assignment Strategy`.


.. _Default Cohort Group:

===========================================================
Ensuring That All Students Are Assigned: The Default Cohort
===========================================================

If you enable cohorts in your course, all students must be assigned to a cohort.
To ensure that there are no students in the course without a cohort, the system
automatically creates a default cohort and assigns students to it if necessary.

The default cohort is created only if you have not created at least one
automated assignment cohort in your course by the time that the first student
accesses your course content. Students who have not been manually assigned to a
cohort when they access the course content are automatically assigned to the
default cohort.

Students who are in the default cohort see a cohort name of "Default Group" in
discussion posts. If you want students to see a different name for the default
cohort, you can change its name. For details about renaming cohorts, see
:ref:`Renaming a Cohort`.

.. image:: ../../../shared/building_and_running_chapters/Images/post_visible_default.png
 :alt: A discussion topic post with "This post is visible to Default Group" 
       above the title

You can check the :ref:`student profile information report<View and download
student data>` for your course to see if any students are assigned to the
default cohort in your course, and change their cohort assignments. Note,
however, that in divided discussion topics students can only see posts by
members of their currently assigned cohort: when a student is reassigned, posts
that he previously saw will seem to have "disappeared". To avoid negatively
affecting the student experience, any cohort assignment changes should be done
as early in the course run as possible, so that students' views of discussion
posts and contributions remain consistent over time.

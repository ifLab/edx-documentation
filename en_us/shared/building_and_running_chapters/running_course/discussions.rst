.. _Discussions:


##################################
管理课程讨论项目
##################################

讨论项目，即论坛，旨在构建学生与工作人员，以及学生与学生之间的有效沟通和交流。
创建课程时，您可设立各种讨论课题引导课程参与人员之间的互动，
同时通过运营、管理讨论项目活动鼓励学生参与课程、建立课程社区。

讨论项目（下或称“论坛”）同时也是课程反馈及未来创意的重要来源。

关于运营、协调讨论项目的内容，请参见以下章节：

* :ref:`Overview_discussions`

* :ref:`Organizing_discussions`

* :ref:`Assigning_discussion_roles`

* :ref:`Visibility of Discussion Topics`

* :ref:`Running_discussions`

* :ref:`Moderating_discussions`

* :ref:`Close_discussions`
  
想了解更多关于分队功能对论坛协调事宜的影响，请参考 :ref:`Moderating Discussions for
Cohorts`.

.. note:: The :ref:`Discussions for Students and Staff` section describes
   features that are available to all discussion participants, and might be
   useful to students who are new to online discussion forums. You can share
   the section with your students by, for example, adding a "Never Used a
   Discussion Forum Before?" post that includes the information you think will
   be most useful to them.


.. _Overview_discussions:

********************************
概述
********************************

学生与员工可以通过论坛分享观点、交流看法、交换意见、解决问题。论坛中的互动分为三种。

*  *帖子* 帖子通常用于展开新话题。帖子一般以问题的形式出现，
  要么展开对话，要么引出一个值得关注的问题。您在发帖时，通常将其归类为“提问”或“讨论”。

*  *回复* 回复指的是关于某个帖子问题的直接回答，或某个对话的延续。

*  *评论* 评论指的是针对某条回复的补充说明或边注。
  评论一般不针对整个帖子，只针对某条回复。
 
由帖子、回复、评论组成的对话有时统称为“话题”。

所有员工及参与课程的学生均可发帖、回帖或发表评论，
同时也可以查看其他课程参与者发布的帖子、回复及评语。

课程社区的所有成员，包括员工和学生，均可以赋予论坛协调员或管理员等讨论项目管理职能。
讨论话题可以保存，是课程历史的组成部分。

.. note:: “参与课堂讨论”一章描述了论坛的部分功能，这些功能对所有参加论坛的人都开放，
   对论坛新人而言帮助也很大。对论坛新人而言帮助也很大。
   您可以和学生一起分享其中的内容。
   方式有很多，比如，您可以发一条名为“第一次使用论坛？”的帖子，
   在帖子中提供您认为对学生最有用的信息。

   Discussion administration roles must be explicitly granted to members of
   the course team for them to moderate or administer course discussions. The
   course author, team members with Admin access (Studio), and Instructors
   (Instructor Dashboard) can grant discussion administration roles. For
   information about adding discussion privileges, see
   :ref:`Assigning_discussion_roles`.


.. _Organizing_discussions:

*************************************************
建立课堂讨论课题
*************************************************

edX课程的论坛既可以添加您之前专门为某个课程单元设计好的讨论模块，
也可以开展全课堂范围的讨论课题，比如“课程反馈帖”，“答疑帖”，“技术支持帖”等等。
您可通过Studio添加各种不同类型的讨论课题。


For more information about creating discussion topics, see :ref:`Create
CourseWide Discussion Topics` and :ref:`Create ContentSpecific Discussion
Topics`. For information about configuring discussion topics in courses that
use cohorts, see :ref:`Set up Discussions in Cohorted Courses`.


.. _Create CourseWide Discussion Topics:

=====================================
创建全课堂讨论课题
=====================================

所有课程均包括一个名为“讨论”的页面。创建课程时，
系统会在该页面中默认生成一个名为“General”的讨论课题。

课堂讨论课题，在课堂上引导学生分享、查找信息。
这类课题可以包含“反馈”、“答疑”、“技术支持”等字样。
这类课题的可访问时间与课程的可访问时间一致。

.. note:: Make sure each discussion topic in your course has a unique name,
   whether it is a course-wide topic or a content-specific discussion topic
   that you add as a discussion component. If different discussion topics
   share the same name, learners might be confused as to which discussion
   topic they are participating in. For example, do not add a content-specific
   discussion topic named "General", because a course-wide discussion topic
   named "General" already exists in every course.

如何创建全课堂讨论课题：

#. 在Studio中打开课程 

#. 单击“设置”→“高级设置”

#. 将滚动滑块拖至“讨论课题映射”策略键。系统默认值应为：

 .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_Add_initial.png
  :alt: Policy value of {"General": {"id": "i4x-edX-Open-edx_demo_course"}}

4. 复制“General”后的三行信息，粘贴到结尾的闭大括号前：

 .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_Add_paste.png
  :alt: Policy value of {"General": {"id": "i4x-edX-Open-edx_demo_course"} 
        "General": {"id": "i4x-edX-Open-edx_demo_course"}}

5. 将第二个“General”替换为新课题的名称，注意带上双引号

#. 将第二个“id”值更改为另一个唯一的值。比如，可以为课题名附上一组独一无二的参数

.. note:: In discussion topic IDs, you can use only alphanumeric characters
   and these special characters: underscore, hyphen, and period.

7. 在第一个闭大括号后输入一个逗号

 .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_Add_name.png
  :alt: Policy value of {"General": {"id": "i4x-edX-Open-edx_demo_course"}, 
        "Course Q&A": {"id": "i4x-edX-Open-edx_demo_course_faq"}}

8. 单击“保存更改”。Studio会重新给您输入的值排序并设定格式。
   将滚动条拖回“讨论课题映射”字段，确认输入内容是否已保存。
   如果您在输入时漏掉了标点符号，输入内容不会保存，且没有警告提示。


操作成功后，当学生单击课程的“讨论”页面时，您的课程即出现在下拉列表中。

 .. image:: ../../../shared/building_and_running_chapters/Images/NewCategory_Discussion.png
  :alt: Image of a new topic named Course Q&A in the list of discussions

.. note:: 在分队课堂中，全课堂讨论课题对所有人均可见。
   所有小队中的学生均可访问课题中的帖子及回复。
   您也可以手动将这类课题配置为分队讨论课题。
   详见 :ref:`Coursewide
   Discussion Topics and Cohorts`.

.. _Create ContentSpecific Discussion Topics:

============================================
Create Content-Specific Discussion Topics
============================================

To create a content-specific discussion topic, you add a discussion component
to a unit. Typically, you do this while you are designing and creating your
course in Studio. Follow the instructions in :ref:`Working with Discussion
Components`. The result is a discussion topic associated with a unit and its
content. 

.. warning:: Follow the recommended steps to add discussion components. Do not
   create discussion topics by using the **Duplicate** button in Studio, and
   do not reference the same discussion ID in more than one place in your
   course. Duplicated discussion components will result in discussion topics
   containing the same conversations, even if learners post in different
   discussion topics.

For more information about the visibility of content-specific discussion
topics, see :ref:`Visibility of Discussion Topics`.

.. note:: In courses with cohorts enabled, all content-specific discussion
   topics are divided by cohort when you first add them. Student posts to divided
   discussion topics can only be read and responded to by members of the same
   cohort. You can change the configuration of content-specific discussion topics
   to make them unified and available to all students in the course. See
   :ref:`Content Specific Discussion Topics and Cohorts`.

.. _Assigning_discussion_roles:

*************************************************
安排讨论项目管理职能
*************************************************

您需要指定一个团队帮助您运营讨论项目。

.. note:: 您在Studio中建立的课程团队（或您在教师控制面板中指定的课程工作人员及导师）
   并不默认为论坛管理人员。


   论坛管理人员应由从课程团队中另外指定，其职责是协调、管理课堂讨论项目。
   论坛管理人员可由课程作者、导师（教师控制面板中的）
   或其他有管理权限的团队成员（Studio中的）担任。


论坛管理人员的分类及职能简述如下：

* *论坛协调员* 论坛协调员可以编辑、删除所有消息（包括帖子、回复、评论）；
  可以审核带有“误用信息”标签的帖子；可以封杀、取消封杀帖子；
  可以将帖子置顶；可以批准回复。在帖子列表中，论坛协调员发布的帖子带有“By:staff”字样，
  协调员发表的回复和评论带有加色的“Staff”标识。
  协调员通常从已担任“课程工作人员”的团队成员中选派。

.. removed this clause from 1st sentence per JAAkana and MHoeber: , and, if the
.. course is cohorted, see posts from all cohorts

* *论坛社区助教* 助教的职能和协调员相同。助教发布的帖子带有“By: Community TA”字样，
  发布的评论和回复带有加色的“Community TA”标识。助教通常由学生担任。

.. I put this comment in to make the formatting of this bulleted list consistent when output using the sphinx template

* *论坛管理员* 拥有以上两种职位的所有职能。
  管理员发布的帖子、回复、评论带有相同的“Staff”标识。
  管理员只能由已担任导师的团队成员出任，
  因为管理员除了具有协调员和助教的只能外，还能在必要的时候赋予其他用户论坛管理职能。


安排论坛管理人员时，您需要提供他们的邮箱地址或用户名。

* 如何查看课程团队成员的信息？在教师控制面板中，单击“成员”，
  然后从下拉列表中选择“课程工作人员”/“导师”。

* 如何查看学生信息？在教师控制面板中，单击“数据下载”
  “以CSV格式下载学生资料”


====================================
如何安排职位
====================================

首先，您必须是课程作者，或担任“导师”职位（即，您必须在Studio中有管理权限）。

#. 查看课程现况

#. 单击“导师”→“成员”

#. 在“行政人员列表管理”字段的下拉列表中选择“论坛管理员”、“论坛协调员”或“论坛社区助教”

#. 在用户列表中输入相应的邮箱地址或用户名，单击“添加”


==============
Remove Roles
==============

To remove role privileges from a user, you must be the course author or
an Instructor (that is, you are identified in Studio as a team member with
Admin access or in the LMS as an Instructor).

#. View the live version of the course.

#. Click **Instructor**, then click **Membership**.

#. In the Administration List Management section, use the drop-down list to
   select Discussion Admins, Discussion Moderators, or Discussion Community
   TAs.

#. From the list of users who currently have that role, select the user you
   want to remove, then click **Revoke access**.


.. _Visibility of Discussion Topics:

**********************************
Visibility of Discussion Topics
**********************************

The names that you specify as the category and subcategory names for
discussion components are not visible on the **Discussion** tab until after
the course has started and the unit is released.

However, "seed" posts that you create in content-specific discussion topics
before a course starts or before the unit is released are immediately visible
on the **Discussion** tab, even though the containing category or subcategory
names are not visible. We recommend that you do not create posts in 
content-specific discussion topics before a unit is released. For more
information about release dates and the visibility of components, see
:ref:`Controlling Content Visibility`.

In contrast, :ref:`course-wide discussion topics<Create CourseWide Discussion
Topics>` that you create on the **Advanced Settings** page in Studio,
including the default "General" discussion topic, are immediately visible,
regardless of whether the course has started. They are not associated with any
particular section or subsection of the courseware, and are not subject to
release dates.


.. _Running_discussions:

*********************
运营讨论项目
*********************

讨论项目管理团队可通过多种方式运营论坛，比如在帖子中作贡献、给回复点赞、
认可某条回复等等，他们通过这些方法引导学生发布与话题相关的消息。
下面的几个小技巧能帮助您有效管理讨论项目。

==========================================
编辑讨论帖主题时采用同一的命名规则
==========================================

为区分不同种类的消息，并使消息更方便查找，
您可以指定一系列命名规则以区分不同种类的帖子主题以及回复、评论。如下例：

* 通知变更事宜时可在帖子主题开头加上“[OFFICIAL]”字样

* 提供错误修复信息的帖子的主题可以用“ERRATA”开头

* 告知学生，如果需要课程工作人员帮助时可以在帖子主题中加入“[STAFF]”字样

讨论项目管理团队和学生均可使用这类命名规则以便更有效地搜索信息。

创建新帖子时，必须选择帖子的类型，是“提问”还是“讨论”。
讨论项目团队成员在选择发帖类型时应慎重，同时也应鼓励学生慎重发帖。详见
:ref:`Find Question Posts and Discussion Posts`.

.. future: changing the type of a post, maybe resequence or separate  conventions from post types

========================
为讨论课题做铺垫
========================

为帮助学生学会如何在课堂讨论中尽可能多地收获知识，
教会学生如何根据自己的问题和讨论寻找最佳的讨论课题，
您可以在课程开始之前发几篇帖子作为课堂讨论的“开胃菜”。示例如下：

* 在“General”课题中，发布一条“[INTRO]”帖子，引导学生和员工做自我介绍。

* 您每发布一个讨论课题，第一条帖子应描述如何使用这个课题。
  除了提供指导教程之外，这类“初始消息”还可作为今后学生创建帖子的范例。

We strongly recommend that you do not create seed posts in content-specific
discussion topics before the course starts or before the containing unit is
released. The category and subcategory names for content-specific discussion
topics are subject to the release visibility of their containing unit, and are
not visible until the unit is released. For more details, see :ref:`Visibility
of Discussion Topics`.


======================================
缩小话题范围
======================================

To encourage longer, threaded discussions rather than many similar, separate
posts, the discussion team can use these techniques. However, be aware that
long threads (with more than 200 responses and comments) can be difficult to
read, and can therefore result in an unsatisfactory experience in the
discussion.

* Pin a post. Pinning a post makes it appear at the top of the list of posts on
  the **Discussion** page. As a result, it is more likely that students will
  see and respond to pinned posts. You can write your own post and then pin it,
  or pin a post by any author. Select the "More" icon and then **Pin**.

    .. image:: ../../../shared/building_and_running_chapters/Images/Pin_Discussion.png
     :alt: Image of the pin icon for discussion posts

* Endorse a response. Endorsing a response indicates that it provides value to
  the discussion. Click the "check mark" (or tick mark) icon for the response.

    .. image:: ../../../shared/building_and_running_chapters/Images/Endorse_Discussion.png
     :alt: Image of the Endorse button for discussion posts

* Mark a question as answered. You use the same procedure to mark a response as
  the correct answer to a question as you do to endorse contributions to a
  discussion: click the "check mark" (or tick mark) icon for correct answers.

* Close a post. You can respond to a redundant post by (optionally) pasting in
  a link to the post that you prefer students to contribute to, and prevent
  further interaction by closing the post. Select the "More" icon and then
  **Close** to close it.

* Provide post/response/comment guidelines. You can post information from the
  :ref:`overview<Overview_discussions>` in this chapter, or the :ref:`anatomy
  of edX discussions<Anatomy of edX Course Discussions>` in the next chapter,
  in a course-wide discussion topic (such as General) to provide guidance about
  when to start a new thread by adding a post, responding to an existing post,
  or commenting on a response.

.. _Moderating_discussions:

***********************
Moderate Discussions
***********************

The members of a course discussion team monitor discussions and keep them
productive. They can also collect information, such as areas of particular
confusion or interest, and relay it to the course staff.

Developing and sustaining a positive discussion culture requires that
sufficient moderator time is dedicated to reviewing and responding to
discussions. Keeping up-to-date with a large MOOC forum requires a commitment
of 5 or more hours per week, and involves reading threads, replying to and
editing posts, and communicating with the rest of the discussion team and
course staff.

For information on setting up moderators for your course, see
:ref:`Assigning_discussion_roles`.

====================================================
View Profile Information for Discussion Participants
====================================================

If you want to find out more about a specific discussion participant, you can
view that learner's edX profile. Learners can have either a limited profile or a
full profile.

To view a learner's profile, follow these steps.

#. On the **Discussion** page, select a username in a post,
   response, or comment.
#. On the **Active Threads** page for that learner, select the
   learner's username.

The following image shows a learner's username in a post, the learner's
username on the **Active Threads** page, and the learner's profile page.

.. image:: ../../../shared/building_and_running_chapters/Images/SFD_Prof_from_Disc.png
  :width: 600
  :alt: Image of a discussion with a learner's username circled, an image of
      that learner's active threads page in the course discussions, and an
      image of the learner's profile

For more information, or to create your own profile, see `View, Create, or
Edit an edX Profile <http://edx- guide-for-
students.readthedocs.org/en/latest/sfd_your_information.html#sfd_pro
file_page>`_.

========================================
Provide Guidelines for Students
========================================

You can develop a set of best practices for discussion participation and make
them available to students as a course handout file or on a defined page in
your course. These guidelines can define your expectations and optionally
introduce features of edX discussions.

You can also share the :ref:`Discussions for Students and Staff` chapter with
your students. It describes features that are available to all discussion
participants, and may be useful to students who are new to online discussion
forums.

.. For a template that you can use to develop your own guidelines, see
.. :ref:`Discussion Forum Guidelines`.

========================================
Develop a Positive Discussion Culture
========================================

Discussion monitors can cultivate qualities in their own discussion
interactions to make their influence positive and their time productive.

* Encourage quality contributions: thank students whose posts have a positive
  impact and who answer questions.

* Check links, images, and videos in addition to the text of each message. Edit
  offensive or inappropriate posts quickly, and explain why.

* Review posts with a large number of votes and recognize "star posters"
  publicly and regularly.

* Stay on topic yourself: before responding to a post, be sure to read it
  completely.

* Maintain a positive attitude. Acknowledge problems and errors without
  assigning blame.

* Provide timely responses. More time needs to be scheduled for answering
  discussion questions when deadlines for homework, quizzes, and other
  milestones approach.

* Discourage redundancy: before responding to a post, search for similar posts.
  Make your response to the most pertinent or active post and then copy its URL
  and use it to respond to the redundant threads.

* Publicize issues raised in the discussions: add questions and their answers
  to an FAQ topic, or announce them on the Course Info page.

For a template that you can use to develop guidelines for your course
moderators, see :ref:`Guidance for Discussion Moderators`.

.. _Find Question Posts and Discussion Posts:

==========================================
Find Questions and Discussions
==========================================

When students create posts, they specify the type of post to indicate whether
they are asking for concrete information (a question) or starting an open-ended
conversation (a discussion). 

On the **Discussion** page, a question mark image identifies posts that ask
questions, and a conversation bubble image identifies posts that start
discussions. When an answer is provided and marked as correct for a question, a
check or tick mark image replaces the question mark image. See :ref:`Answer
Questions`.

In addition to these visual cues, filters can help you find questions and
discussions that need review. Above the list of posts on the **Discussion**
page, the **Show all** filter is selected by default. You can also select:

* **Unread**, to list only the discussions and questions that you have not yet
  viewed.

* **Unanswered**, to list only questions that do not yet have any responses
  marked as answers.

==================
Edit Messages
==================

Discussion moderators, community TAs, and admins can edit the content of posts,
responses, and comments. Messages that include spoilers or solutions, or that
contain inappropriate or off-topic material, should be edited quickly to remove
text, images, or links.

#. Log in to the site and then select the course on your **Current Courses**
   dashboard.

#. Open the **Discussion** page and then open the post with the content that
   requires editing. You can select a single topic from the drop-down list of
   discussion topics, apply a filter, or search to locate the post.

#. For the post or for the response or comment that you want to edit, click the
   "More" icon and then **Edit**.

#. Remove the problematic portion of the message, or replace it with standard
   text such as "[REMOVED BY MODERATOR]".

#. Communicate the reason for your change. For example, "Posting a solution
   violates the honor code."

==================
Delete Messages 
==================

Discussion moderators, community TAs, and discussion admins can delete the
content of posts, responses, and comments. Posts that include spam or abusive
language may need to be deleted, rather than edited.

#. Log in to the site and then select the course on your **Current Courses**
   dashboard.

#. Open the **Discussion** page and then open the post with the content that
   requires deletion. You can select a single topic from the drop-down list of
   discussion topics, apply a filter, or search to locate the post.

#. For the post or for the response or comment that you want to delete, click
   the "More" icon and then **Delete**.

#. Click **OK** to confirm the deletion.

.. how to communicate with the poster?

.. important:: If a message is threatening or indicates serious harmful 
 intent, contact campus security at your institution. Report the incident
 before taking any other action.

==================================
Respond to Reports of Misuse
==================================

Students have the option to report contributions that they find inappropriate.
Moderators, community TAs, and admins can check for messages that have been
flagged in this way and edit or delete them as needed.

#. View the live version of your course and click **Discussion** at the top of
   the page.

#. In the list of posts on the left side of the page, use the filter drop-down
   list (set to **Show all** by default) to select **Flagged**.

#. Review listed posts. A post is listed if it or any of its responses or
   comments has been reported. The reported contribution includes a
   **Reported** identifier.

#. Edit or delete the post, response, or comment. Alternatively, remove the
   flag: click the "More" icon and then **Unreport**.

===============
Block Users
===============

For a student who continues to misuse the course discussions, you can unenroll
the student from the course. See :ref:`unenroll_student`. If the enrollment
period for the course is over, the student cannot re-enroll.

.. _Close_discussions:

******************************
Close Discussions
******************************

You can close the discussions for your course so that students cannot add
messages. Course discussions can be closed temporarily, such as during an exam
period, or permanently, such as when a course ends.

When you close the discussions for a course, all of the discussion topics in
course units and all of the course-wide topics are affected.

* Existing discussion contributions remain available for review.
  
* Students cannot add posts, respond to posts, or comment on responses.
  However, students can continue to vote on existing threads, follow threads,
  or report messages for misuse.

* Course Staff, Instructors, Discussion Admins, Discussion Moderators,
  and Discussion Community TAs are not affected when you close the discussions
  for a course. Users with these roles can continue to add to discussions. 

.. note:: To make sure your students understand why they cannot add to 
  discussions, you can add the dates that discussions are closed to the
  **Course Info** page and post them to a General discussion.

=====================================
Start-End Date Format Specification
=====================================

To close course discussions, you supply a start date and time and an end date
and time in Studio. You enter the values in this format:

``["YYYY-MM-DDTHH:MM", "YYYY-MM-DDTHH:MM"]``

where:

* The dates and times that you enter are in the Universal Coordinated (UTC)
  time zone, not in your local time zone.

* You enter an actual letter **T** between the numeric date and time values. 

* The first date and time indicate when you want course discussions to close.

* The second date and time indicate when you want course discussions to reopen.

* If you do not want the discussions to reopen, enter a date that is far in the
  future.

* Quotation marks enclose each date-time value.

* A comma and a space separate the start date-time from the end date-time.

* Square brackets enclose the start-end value pair.

* You can supply more than one complete start and end value pair. A comma and a
  space separate each pair.

For example, to close course discussions temporarily for a final exam period in
July, and then permanently on 9 August 2014, you enter:

``["2014-07-22T08:00", "2014-07-25T18:00"], ["2014-08-09T00:00", "2099-08-09T00:00"]``

You enter these values between an additional pair of square brackets which are
supplied for you in Studio.

============================================
Define When Discussions Are Closed
============================================

To define when discussions are closed to new contributions and when they
reopen:

#. Open your course in Studio. 

#. Select **Settings**, then **Advanced Settings**.

#. Scroll down to the **Discussion Blackout Dates** policy key. 

#. In the field for the value, place your cursor between the supplied square
   brackets. Use the required date format specification to enter the start and
   end dates for each time period during which you want discussions to be
   closed.

   When you enter the dates and times from the example above, the value field
   looks like this:

   .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_blackout_unformatted.png
     :alt: Policy value of [["2014-07-22T08:00", "2014-07-25T18:00"],
         ["2014-08-09T00:00", "2099-08-09T00:00"]]

5. Click **Save Changes**.

   Studio reformats your entry to add line feeds and indentation, like this:

   .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_blackout_formatted.png
     :alt: Same policy value but with a line feed after each bracket and comma,
         and an indent before each date

For examples of email messages that you can send to let students know when the
course discussions are closed (or open), see :ref:`Example Messages to
Students`.

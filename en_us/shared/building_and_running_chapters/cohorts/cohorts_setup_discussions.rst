
.. _Set up Discussions in Cohorted Courses:


######################################################
在包含队列的课程中设置论坛
######################################################

在开启了队列的课程中，讨论主题可以按队列分类或统一对所有学生可见。
按队列分类的讨论主题对所有学生可见，但是帖子、回复和评论仅对队列成员可见。
统一讨论主题中的帖子、回复和评论对所有学生可见。

当您第一次在课程中开启队列时，
:ref:`course-wide discussion topics<Coursewide Discussion Topics and Cohorts>` 
的初始设定和 :ref:`content-specific discussion topics
<Content Specific Discussion Topics and Cohorts>` 的设定不同。

默认状态下，全课堂讨论主题是统一的，因为这些讨论一般是为课程中的所有学生都感兴趣的内容设置的。
相反，内容指定讨论主题是默认按队列分配的。在导师面板中，您可以更改讨论主题的类型。

.. warning:: 如果您在学生开始阅览和贡献讨论帖时，更改在线课程中讨论主题的队列设置，
   您将更改学生的课程体验。学生可能看到之前看不到的帖子，或者看不到以前能看到的帖子。
   如果您更改任何已开始课程的设置，请注意改变可能造成的影响。更多细节请参阅 :ref:`Altering Cohort Configuration` 。

关于讨论主题的队列设置，请参考以下主题。

* :ref:`Coursewide Discussion Topics and Cohorts`
* :ref:`Specify Whether CourseWide Discussion Topics are Cohorted`
* :ref:`Content Specific Discussion Topics and Cohorts`
* :ref:`Specify that All ContentSpecific Discussion Topics are Cohorted`
* :ref:`Specify Some ContentSpecific Discussion Topics as Cohorted`

关于课程论坛的概览请参阅 :ref:`Discussions`.
关于使用队列和管理按队列分类讨论的信息请参考 :ref:`Cohorts Overview` and :ref:`Moderating
Discussions for Cohorts`.

.. note:: 本章和以下主题中描述的按队列分类讨论主题，只能将讨论主题中的帖子进行分类，
   讨论主题本身还是对所有学生可见。如果您想设置指定内容讨论主题尽对特定队列可见，
   您可以使用内容小组并更改讨论组件的可见性设置。具体细节请参阅 :ref:`Cohorted Courseware Overview`.


.. _Coursewide Discussion Topics and Cohorts:

***********************************************
全课堂讨论主题和队列
***********************************************

当您第一次 :ref:`create a course-wide discussion topic<Create CourseWide
Discussion Topics>` 时，该主题是统一的，课程内的所有学生都可以发帖、
阅览帖子、回复和评论。

在您添加了全课堂主题后，您可以使其按队列分类。
设定全课堂讨论主题属性的相关内容请参考 :ref:`Specify Whether
CourseWide Discussion Topics are Cohorted`.

====================================================================
示例：按队列分类全课堂讨论主题
====================================================================

全课堂讨论主题是默认为统一属性，所以所有学生都能参与讨论。
某些情况下，您可能决定按队列分类全课堂讨论主题，
这样每个队列中的成员只能看到同队列中成员的回复和发帖。

例如，除系统自带“一般性说明”主题之外，您添加了三个新的全课堂讨论主题，一共为四个主题。

* 一般性说明
* 课程 Q&A
* 声明
* 头脑风暴

您在一般性说明和课程Q&A主题中，以及其他您希望学生探索的课题中发布的帖子适用于所有学生。
但是您决定将声明和头脑风暴按队列分类。关于指定全课程讨论主题是否按队列分类的信息，
请参考 :ref:`Specify Whether CourseWide Discussion Topics are
Cohorted`.

您也可以使用命名对话，学生在发帖前可以了解该讨论主题的受众。
更多关于命名对话的信息请参考 :ref:`Apply Naming Conventions to Discussion
Topics`.


.. _Specify Whether CourseWide Discussion Topics are Cohorted:

********************************************************************
指定全课堂讨论主题是否按队列分类
********************************************************************

当您 :ref:`create course-wide discussion topics<Create CourseWide
Discussion Topics>` 时， 主题默认为统一属性，所有学生都能看见并回复其他学生的帖子。
您可以更改全课堂讨论主题设置，将其按队列分类，这样学生只能看到相同队列中成员的回复和发帖。

按照以下步骤更改全课堂讨论主题的队列设置。

#. 在学习管理系统中选择 **导师** ，选择 **队列** 。

#. 点击 **指定讨论主题是否按队列分类** 。
   
#. 在 **全课程讨论主题** 一节，勾选您想划分的主题。
   
#. 点击 **保存** 。
   
   全课堂讨论主题列表更新。

.. image:: ../../../shared/building_and_running_chapters/Images/CohortDiscussionsCourseWide.png
  :alt: Two course-wide discussion topics in list, one cohorted and one unified

更多关于管理按队列分类的讨论主题请参考
:ref:`Moderating Discussions for Cohorts`.


.. _Content Specific Discussion Topics and Cohorts:

**********************************************
指定内容讨论主题和队列
**********************************************

当您开启了队列，并通过在Studio单元中添加讨论组件 :ref:`create content-specific
discussion topics<Create ContentSpecific Discussion Topics>`  后，
这些指定内容讨论主题默认按队列分类。
学生只能看到本队列成员发布的帖子、回复以及评论。

如果您想让所有指定内容讨论主题按队列分类，您不需要做任何操作。
更多信息请参考 :ref:`Specify that All ContentSpecific Discussion Topics are Cohorted`.

您也可以选择指定大多数指定内容讨论主题为统一属性，然后设置 :ref:`only a few
discussion topics divided by cohort<Specify Some ContentSpecific Discussion
Topics as Cohorted>`.


.. _Specify that All ContentSpecific Discussion Topics are Cohorted:

*****************************************************************
设置所有指定内容讨论主题按队列分类
*****************************************************************

The default behavior for content-specific discussion topics is that they are
divided by cohort when you first :ref:`add them<Create ContentSpecific
Discussion Topics>` in your courseware. If you want all content-specific
discussion topics in your course to be divided by cohort, you do not need to
take any action.

You can confirm this setting on the Instructor Dashboard **Cohorts** tab. 

#. In the LMS, select **Instructor**, then select **Cohorts**. 

#. Click **Specify whether discussion topics are divided by cohort**. 

.. image:: ../../../shared/building_and_running_chapters/Images/CohortDiscussionsSpecifyLink.png
 :alt: The link in the UI to specify whether content specific discussion topics are divided by cohort
   
In the **Content-Specific Discussion Topics** section, you see that the
**Always cohort content-specific discussion topics** option is selected. 

All content-specific discussion topics in your course are divided by cohort,
and you cannot change the cohort settings of individual content-specific
discussion topics.

.. image:: ../../../shared/building_and_running_chapters/Images/CohortDiscussionsAlwaysCohort.png
 :alt: Content specific discussion topics controls with the "Always cohort
  content specific discussion topics" option selected

For information about changing the cohort settings for your content-specific
discussions to make all of them unified except a few, see :ref:`Specify Some
ContentSpecific Discussion Topics as Cohorted`.


.. _Specify Some ContentSpecific Discussion Topics as Cohorted:

**************************************************************************
Specify that Some Content-Specific Discussion Topics are Divided by Cohort
**************************************************************************

The default behavior for content-specific discussion topics is that they are
divided by cohort when you first :ref:`add them<Create ContentSpecific
Discussion Topics>` in your courseware.

To make only a few of your content-specific discussion topics divided by
cohort, you change the cohort settings for content-specific discussion topics
to make them all unified, and then explicitly select only the topics that you
want to be divided by cohort.

.. warning:: When you change the cohort setting from **Always Cohort Content-Specific
   Discussion Topics** to **Cohort Selected Content-Specific Discussion Topics**, 
   you are making all content-specific discussion topics in your course unified, unless
   you explicitly change them to be divided by cohort before saving your changes. 
   This means that any posts that were previously divided by cohort and restricted to 
   viewing, responding, and commenting by members of the same cohort are now visible
   to all learners in your course. 

   If you make changes to cohort settings in a running course, be aware of the
   implications of your changes. For more details, see :ref:`Altering Cohort
   Configuration`.


To specify that only some content-specific discussion topics in your course are
divided by cohort, follow these steps.

#. In the LMS, select **Instructor**, then select **Cohorts**. 

#. Click **Specify whether discussion topics are divided by cohort**. 

.. image:: ../../../shared/building_and_running_chapters/Images/CohortDiscussionsSpecifyLink.png
 :alt: The link in the UI to specify whether content specific discussion topics are divided by cohort
   
3. In the **Content-Specific Discussion Topics** section, if it is not already
   selected, select **Cohort selected content-specific discussion topics**.
   
   .. warning:: If you make changes to cohort settings in a running course, be
      aware of the implications of your changes. For more details, see
      :ref:`Altering Cohort Configuration`.

   All content-specific discussion topics that you add in your course are
   unified and visible to all learners. The list of content-specific
   discussion topics becomes editable.
   
#. Select the checkbox next to each content-specific discussion topic that you
   want to divide by cohort.

   .. image:: ../../../shared/building_and_running_chapters/Images/CohortDiscussionsCohortSelected.png
     :alt: Content specific discussion topics controls with the "Cohort
      selected content specific discussion topics option selected
   
#. Click **Save**.
   
   The changes to your content-specific discussions are saved. The content-specific
   discussion topics that you selected are saved as being divided by cohort. All other
   content-specific discussion topics are unified.

For more information about managing discussions that are divided by cohort, see
:ref:`Moderating Discussions for Cohorts`.


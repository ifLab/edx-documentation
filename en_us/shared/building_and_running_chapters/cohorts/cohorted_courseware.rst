.. _Cohorted Courseware Overview:


###################################
创建特定队列课件
###################################

如果您在课程中已经 :ref:`cohorts enabled<Enabling and Configuring Cohorts>` ，
您可以为不同队列的学生提供不同的课程体验。

您可以使一些学生得到的内容与其他学生不同。
您可以在Studio中建立 :ref:`content groups<About Content Groups>` ，
将特定组件设定为仅对一个或多个内容小组可见。
如果您将一个或多个队列结合到同一个内容小组中，
只有这些队列中的成员能够看到您设定的内容。

更多关于内容小组的内容请参考 :ref:`About Content Groups` 。 
关于特定内容队列的示例请参考 :ref:`Cohorted Courseware
Example`.


完成以下步骤创建特定队列内容：

在Studio中：

#. :ref:`Enable cohorts in your course<Enabling and Configuring Cohorts>`.
#. :ref:`Create content groups<Creating Content Groups>`. 
#. :ref:`Specify components in courseware as visible only to particular content
   groups<Specify Components in Courseware as Visible Only to Certain Content
   Groups>`.
     
在学习管理系统中： 

#. :ref:`Assign students to cohorts<Options for Assigning Students to Cohorts>`.  
#. :ref:`Associate one or more cohorts with a content group<Associate Cohorts
   with Content Groups>`.
#. :ref:`Preview cohort-specific courseware<Preview Cohort Specific Courseware>`.


.. _Cohorted Courseware Example:

***********************************
示例：特定队列课件
***********************************

假设您在课程中建立了两个 :ref:`cohorts<Cohorts Overview>` ，
大学校友和大学在校生。当学生进入课件页面或论坛中时，
不在这两个队列中的学生被自动分配到第三个队列中，即默认队列。
更多关于在课程中启动队列和分派队列的信息请参考 :ref:`Enabling and Configuring Cohorts` 。

除了两个学校相关的队列的学生将得到他们感兴趣的特殊内容以外，您希望其他所有的学生将到相同的课程体验。

在每个章节最后，您希望包含一个来自学校官方，包括校长和学院院长的视频信息。
这些视频仅向您学校的学生和校友展示。在每章节的最后，您想测验一下本章节的知识。
这些测验题仅对所有参加本课程的学生可见。

要达到这些要求，在Studio的 **小组设置** 页面中建立名为“学校特别内容”内容小组。
在导师界面的 **队列** 栏中，将“校友”和“在校学生”队列合并到“学校特别内容”小组中。

在您的课程大纲页面，更改视频组件的可见性设置，
使各章节末尾的视频仅对“学校特别内容”内容小组可见。
您不需要改变小测试题的可见性，因为如果没有在组件可见性设置中特定内容小组，
组件将对所有学生可见。


As a final step, you preview the course in the LMS to ensure that students see
the content that is intended for them. You confirm that when you view the course
in the role of **Student** (in other words, any student not in a content group),
you see a quiz at the end of each section, but do not see the university-related
videos. When you view the course as a student in the "University-Specific
Content" group, you see a university-related video as well as the quiz at the
end of each section.


.. _About Content Groups:

**************
Content Groups
**************

Content groups are virtual groupings of students who will see a particular set
of course content. You can use content groups to designate specific course
content as visible to particular :ref:`cohorts<Cohorts Overview>` of students. 

You create content groups in Studio, and in your course outline you use the
**Visibility Settings** to designate whether a component is selectively visible
only to one or more content groups. Any course components that do not have an
explicitly restricted visibility setting remain visible to all students,
regardless of their cohort.

Content groups do not have an actual impact on the visibility of a course
component until you associate them with one or more cohorts. If you have
designated certain course content as visible to a content group, and in addition
have associated that content group with one or more cohorts, then those cohorts
will see the designated content.

For an example of using content groups to create cohort-specific courseware, see
:ref:`Cohorted Courseware Example`.


.. _Creating Content Groups:

*********************
Create Content Groups
*********************

To create a content group, follow these steps.

#. In Studio, select **Settings**, then select **Group Configurations**.
 
#. On the **Group Configurations** page, click **New content group**.
   
.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_AddContentGroup.png
 :width: 600
 :alt: Button on Group Configurations page for adding first content group

3. Enter a meaningful name for the content group, then click **Create**.
   The page refreshes to show the name of your new content group.
#. Repeat this step to create as many content groups as you want.

After you create a content group, you can work with your course outline to
specify which components are visible to specific content groups. For details,
see :ref:`Specify Components in Courseware as Visible Only to Certain Content
Groups`.

On the Instructor Dashboard, you associate each content group with one or more
cohorts. For details, see :ref:`Associate Cohorts with Content Groups`.


.. _View Usage of a Content Group:

*************************************
View Usage of a Content Group
*************************************

To view the units that are visible to a content group, follow these steps.

#. In Studio, select **Settings**, then select **Group Configurations**.
 
#. On the **Group Configurations** page, locate the content group for which you
   want to view the usage.
   
   The content group's box displays whether the content group is used in this
   course. If it is used, you see the number of units that it is used in, and
   links to each unit.

#. Click each link to go to that unit in the **Course Outline**, where you can
   :ref:`specify whether that unit is visible to the content group<Specify
   Components in Courseware as Visible Only to Certain Content Groups>`.

For details about previewing your course to ensure that students in a cohort
correctly see the content intended for them, see :ref:`Preview Cohort Specific
Courseware`. For details about deleting content groups, see :ref:`Delete Content
Groups`.


.. _Delete Content Groups:

*********************
Delete Content Groups
*********************

.. note:: You can delete a content group only if it is not in use in any course
   unit. To delete a content group that is currently in use, you must first
   remove it from any course unit visibility settings that use the content
   group. For information about seeing which units use a content group, see
   :ref:`View Usage of a Content Group`.

#. In Studio, select **Settings**, then select **Group Configurations**.
 
#. On the **Group Configurations** page, locate the content group that you want
   to delete.  
   
#. Move your cursor over the content group's box, then click the **Delete**
   icon.

#. In the confirmation message, click **Delete** again to confirm the deletion.
      

.. _Specify Components in Courseware as Visible Only to Certain Content Groups:

*****************************************************************************
Specify Components in Courseware as Visible Only to Particular Content Groups
*****************************************************************************

After you create at least one content group, you can edit your course in Studio
and modify the visibility settings of components that you want to make visible
only to particular content groups.

.. note:: You do not need to edit the visibility settings of components that are
   intended for all students. Components that you do not explicitly indicate as
   visible to a group are visible to all students enrolled in your course,
   regardless of the cohort that they belong to.

You can specify content as visible to content groups only at the component level
in a unit. You cannot specify entire units, subsections, or sections for
visibility to content groups.

In a separate task, you create cohorts and associate content groups with
cohorts. Then, only the cohorts associated with content groups which you
selected in a component's visibility settings can view the component. See
:ref:`Associate Cohorts with Content Groups` for details about associating
cohorts with content groups.

To specify components as visible only to particular content groups, follow these
steps.

#. In Studio, select **Content**, then select **Outline**. 
   
#. For each component that you want to make visible only to a particular
   content group or groups, click the unit name, then click the **Visibility
   Settings** icon.

.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_VisibilitySettingInUnit.png
  :alt: Screen capture of unit in course outline with visibility setting icon highlighted 

3. In the **Editing visibility** dialog, select **Specific Content Groups**,
   then select the checkbox for each content group for which you want the current
   component to be visible.

.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_EditVisibility.png
  :width: 400
  :alt: Screen capture of unit in course outline with visibility setting icon highlighted 

4. Click **Save**.

The **Visibility Settings** icon for the component is now black, and the
publishing details for the course section in the sidebar refresh to indicate
that some content is visible only to particular groups.

.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_VisibilitySomeGroup.png
   :alt: Visibility icon is black when visibility for a component is restricted

.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_OnlyVisibleToParticularGroups.png   
   :alt: Course outline sidebar shows visibility icon and note indicating that some content in the unit is visible only to particular group.

For details about previewing your course to ensure that students in a cohort
correctly see the content intended for them, see :ref:`Preview Cohort Specific
Courseware`.

.. note:: In addition to visibility settings for content groups, a student's
   ability to see a course component also depends on whether it is hidden from
   students, whether the unit is published, and the course's release date. For
   details about previewing courseware in general, see :ref:`Preview Course
   Content`.

.. _Associate Cohorts with Content Groups:

*************************************
Associate Cohorts with Content Groups
*************************************

After you create a content group, you can associate it with one or more cohorts
with which you want to share the same special content in your course.

.. note:: A content group can be associated with more than one cohort; a cohort
   cannot be associated with more than one content group.

To associate a cohort with a content group, follow these steps:

#. In the LMS, select **Instructor**, then select **Cohorts**. 
   
#. From the cohorts drop down list, select the cohort to which you want to
   associate your content group.
   
#. Click the **Settings** tab for the selected cohort.

#. Under **Associated Content Group**, choose the **Select a Content Group** option.

#. From the content group drop down list, select the content group that you want
   your cohort to be associated with.

.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_AssociateWithContentGroup.png
   :alt: Select a content group to associate with the cohort

7. Click **Save**.
   
   You have now associated your content group with a cohort. Any course content
   that you :ref:`designate as visible to that content group<Specify Components
   in Courseware as Visible Only to Certain Content Groups>` is visible to
   students in the associated cohort or cohorts.

You can associate additional cohorts with the same or a different content group
by repeating steps 3 to 7.

For an example of using content groups to create cohort-specific courseware, see
:ref:`Cohorted Courseware Example`.


.. _Preview Cohort Specific Courseware:

*************************************
Preview Cohort-Specific Courseware
*************************************

After you designate components in your course as being visible only to certain
content groups, you can preview your courseware to ensure that each group
correctly sees the content intended for them.

.. note:: In addition to visibility settings for content groups, a student's
   ability to see a course component also depends on whether it is hidden from
   students, whether the unit is published, and the course's release date. For
   details about previewing courseware in general, see :ref:`Preview Course
   Content`.

You can view the course as a member of these groups:


.. list-table::
    :widths: 15 30
    :header-rows: 1

    * - Role
      - When You "View As" This Role
    * - Staff
      - You see all content in the course, including content
        that is hidden from students.
    * - Student
      - You see any content that is intended for all
        students.
    * - Student in <Content Group Name>            
      - You see content that is intended for all students, as well
        as any content specifically set to be visible to this content group.

#. In Studio, in the course outline, click **Preview**. You see your
   course section in the **Courseware** section of the LMS.

#. In the navigation bar at the top of the page, select one of the options in
   the **View this course as** drop down list, as described in the table above.

.. image:: ../../../shared/building_and_running_chapters/Images/Cohorts_ViewCourseAs.png
   :alt: Visibility icon is black when visibility for a component is restricted


The course view refreshes and the content is presented as a member of the
selected content group would see it.

After your course is live, you can also see the live version as a student would
see it, by clicking **View Live** from Studio. For more information, see
:ref:`View Your Live Course`.



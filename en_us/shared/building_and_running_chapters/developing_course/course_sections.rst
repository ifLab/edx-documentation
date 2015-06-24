.. _Developing Course Sections:

###################################
创建课程章节
###################################

创建课程章节之前，您必须了解以下内容：

* `What is a Section?`_
* `Viewing Sections in the Outline`_
* `The Student View of a Section`_
* `Sections and Visibility to Students`_
* `Release Statuses of Sections`_

  
创建章节时需完成的任务:

* `Create a Section`_
* `Change a Section Name`_
* `Set a Section Release Date`_
* `Publish all Units in a Section`_
* `Hide a Section from Students`_
* `Delete a Section`_


****************************
什么是章节？
****************************

章节应是课程目录中的第一级标题。
一个章节可以表示一段时间，一章内容或其他组织形式。
一个章节应包含一个或多个小节。

********************************
在课程大纲中预览章节
********************************

下图显示了大纲中四个收起的章节：

.. image:: ../../../shared/building_and_running_chapters/Images/sections-outline.png
 :alt: Four sections in the outline

******************************
学生界面中的章节
******************************

学生可以在课件库中查看章节，并可以通过展开章节查看全部内容。
如下图所示，方框中有三个章节，其中第三个章节展开了所有的小节内容：

.. image:: ../../../shared/building_and_running_chapters/Images/sections_student.png
 :alt: The students view of the course with two sections circled

************************************************
章节对学生的可见性
************************************************

学生无法看见任何尚未发布或者已过发布期限的章节。

如果出现下列情况，学生仍然可以看见已过发布日期的内容：

* 包含次容的章节已经过了发布日期。
* 已经发布的目标单元。
* 未对学生隐藏的单元。

************************************************
章节的发布状态
************************************************

课程制作者可以控制各个章节的发布状态。学生只能看见发布的章节，了解章节的发布状态，请参考以下信息：

* `Unscheduled`_
* `Scheduled`_
* `Released`_
* `Released with Unpublished Changes`_
* `Staff Only Content`_

========================
尚未设置发布时间
========================

如果您在创建新章节时没有修改 :ref:`course start date<Set Start and End Dates>`
默认开始时间 ``1/1/2030 00:00:00 UTC``，那么该章节的发布日期会显示为 ``Unscheduled`` 。
处于这种状态下，学生无法看见该章节中的任何内容，不管该部分内容是否发布。

如果您在创建新章节时修改了课程开始时间，那么该日期就是课程开始的时间

下图用灰条表明了尚未设置发布日期的章节在课程大纲中是如何显示的。

.. image:: ../../../shared/building_and_running_chapters/Images/section-unscheduled.png
 :alt: An unscheduled section

为确保内容对学生可见，请您务必设置发布日期。

==============
已设置发布时间
==============

无论章节中的内容是否发布，学生都只能看见处于发布日期中的章节。

下图用绿条表明了设置了发布日期的章节在课程大纲中是如何显示的。

.. image:: ../../../shared/building_and_running_chapters/Images/section-future.png
 :alt: An section scheduled to release in the future

章节只有在到达发布日期后才能对学生显示。

===========================
已发布
===========================

学生可以看见已经发布的章节；但是，并不能看见章节中的所有内容，只有已经发布的小节或者单元才对学生显示。

图中，蓝色线处列出了发布章节在大纲中是如何显示的。

.. image:: ../../../shared/building_and_running_chapters/Images/section-released.png
 :alt: An unscheduled section

==================================
已发布的内容中含有未发布的修改
==================================

如果您修改了发布章节中的一个单元，但是没有对修改进行重新发布，那么学生是无法看见最新版本的。

下图黄色区域列举了尚未发布的更改是如何在大纲中显示的：

.. image:: ../../../shared/building_and_running_chapters/Images/section-unpublished-changes.png
 :alt: A section with unpublished changes

您必须重新发布更改信息才能对学生可见

===========================
仅对教员开放的内容
===========================

无论发布与否，学生无法看见仅对教员开放的单元。

下图黑色区域列举了仅对教员开放的单元是如何在大纲中显示的。

.. image:: ../../../shared/building_and_running_chapters/Images/section-hidden-unit.png
 :alt: A section with a hidden unit 


.. _Create a Section:

****************************
创建章节
****************************

如果您在创建新章节时没有修改 :ref:`course start date<Set Start and End Dates>`
的默认开始时间 ``1/1/2030``，那么该章节的发布日期会显示为 ``Unscheduled`` 。

如果您在创建新章节时修改了课程开始时间，那么该日期默认为课程开始时间。

.. caution:: 
  如果将课程开始时间设置为过去的时间，那么课程建好后学生就可以访问了。

如何创建章节：

#. 在课程大纲的头部或者底部，单击 **新章节** 。 
   
   .. image:: ../../../shared/building_and_running_chapters/Images/outline-create-section.png
     :alt: The outline with the New Section buttons circled

   新建章节会出现在课程内容的末端，并提示选择章节名称。
   

#. 输入新章节的名称。描述性的名称能帮助学生在课件中找到内容，
   也帮助您在edX Insights分析绩效时选择内容。


#. 您也可以为新建章节 :ref:`Add subsections<Create a Subsection>` 
   
我们建议您在创建章节时 :ref:`test course content <Testing Your Course
Content>` 。

********************************
更改章节名称
********************************

将鼠标悬停在章节名称上直至出现“编辑”按钮：

.. image:: ../../../shared/building_and_running_chapters/Images/section-edit-icon.png
  :alt: The Edit Section Name icon

点击“编辑”按钮，输入新的名称；

.. _Set a Section Release Date:

********************************
设置章节的发布日期
********************************

按照以下步骤设置章节发布日期：

#. 点击章节中的“设置”按钮
   
   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-box.png
    :alt: The section settings icon circled

   打开 **设置** 对话框

#. 输入章节的发布日期和时间：
   
   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-release-date.png
    :alt: The section release date settings

#. 点击 **保存**

欲了解更多信息，请查看 :ref:`Release Dates`.

.. _Publish all Units in a Section:

********************************
发布章节中的所有单元
********************************

点击章节中的“发布”按钮，发布新建及修改的单元：

.. image:: ../../../shared/building_and_running_chapters/Images/outline-publish-icon-section.png
 :alt: Publishing icon for a section

.. note:: 
 只有对章节做出修改后，才会出现“发布”按钮。

有关单元发布状态及对学生可见性等相关信息，请查看 :ref:`Unit Publishing Status` 。


.. _Hide a Section from Students:

********************************
对学生隐藏章节
********************************

无论章节中的小节、单元发布状态如何，您都可以对学生隐藏所有内容。

更多内容请参阅 :ref:`Content Hidden from Students`。

如何对学生隐藏章节内容：

#. 点击“设置”按钮。
   
   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-box.png
    :alt: The section settings icon circled

   弹出 **设置对** 话框。

#. 点击 **对学生隐藏** 按钮。

   .. image:: ../../../shared/building_and_running_chapters/Images/section-settings-hide.png
    :alt: The section hide from students setting

#. 点击 **保存** 。

至此，所有内容都对学生隐藏了。

要对学生开放此章节，只需重复以上步骤，清除 **对学生隐藏** 复选框。

.. warning::
清除 **对学生隐藏** 复选框并不会将所有内容呈现给学生，特别是单独设置了对学生隐藏的小节、单元，及尚未发布的内容。

********************************
删除章节
********************************

删除章节就是删除章节里包含的所有内容。


.. warning::  
  删除的课程内容无法恢复。您可以将暂时不用的课程内容存放在一个章节中，并将该章节设置成“永不发布”。

如何删除章节：

#. 点击章节中的“删除”按钮：

  .. image:: ../../../shared/building_and_running_chapters/Images/section-delete.png
   :alt: The section with Delete icon circled

2. 在弹出的确认对话框中选择“是”即可删除该章节。

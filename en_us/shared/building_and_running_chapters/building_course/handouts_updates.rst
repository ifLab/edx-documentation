.. _Adding Course Updates and Handouts:

######################################################
添加课程补充资料及讲义
######################################################

在Studio中，您可以添加课程的补充资料或讲义。
在 **课程信息** 选项卡下，学生可查看补充资料或讲义。

.. image:: ../../../shared/building_and_running_chapters/Images/course_info.png
 :alt: The Course Info page as it appears to students, with a "Course Updates
       & News" section containing a dated post and a "Course Handouts" frame
       with a list of links.

.. contents:: Section Contents 
   :local:
   :depth: 1

.. _Add a Course Update:

**********************
如何添加课程补充资料
**********************

您可添加课程的补充资料，通知学生考试、课程表变更或是其他突发情况。

如何添加补充资料：

#. 在 **内容** 菜单中，选择 **更新** 。 
#. 单击 **新资料** 。
#. 在打开的HTML编辑器中输入内容。

   * 内容必须是HTML格式，不提供 :ref:`visual editor<The
     Visual Editor>` 格式。
   * 如果您更改了补充日期，新的日期会在 **课程信息** 中显示。
     然而，一经上传，资料对所有已登记学生可见。

4. Select **Post**. Your update appears on your course's **Course Info** page
   immediately.

.. _Add Course Handouts:

***************************
添加讲义
***************************

您可以使用先前上传的文件作为课程讲义。
学生可以在 **课程信息** 页面看到所有课程讲义的链接。

在添加课程讲义之前，您需要 :ref:`add the file<Add Files to a Course>` 到您的课程中并复制文件的Studio URL。
为简化操作，您可以在另一个浏览器窗口中打开Studio中的 **文件与上传** 页面。

如何添加课程讲义：

#. 在 **内容** 菜单中，选择 **补充材料**
#. 在 **课程讲义** 选项卡下，选择 **编辑**
#. 在打开的编辑器中，用HTML格式添加之前上传的文件地址链接。
   示例如下：

   .. code-block:: html

     <p><a href="/static/Syllabus_Fall2016.pdf" target="_blank">Syllabus</a></p>
     <p><a href="/static/Glossary_v3.pdf" target="_blank">Glossary</a></p>

4. 单击 **保存**

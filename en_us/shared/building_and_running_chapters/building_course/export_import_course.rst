.. _Exporting and Importing a Course:

#####################################
输出和导入课程
#####################################

您可以通过Studio :ref:`Export a Course` 和 :ref:`Import a Course`  

您将使用 :ref:`.tar.gz files <Work
with the targz file>`对课程进行导入和输出。

复制并重新开设已有的课程，请选择课程重开选项。详情请参考 :ref:`Rerun a Course`.

.. caution::
  在输出和导入课程之前，请确保课程间的链接使用 ``/jump_to_id/<unit identifier>`` 语法。 
  如果未使用 ``/jump_to_id/<unit identifier>`` 语法， 您在输出再导入课程时链接会失效。
  详情请参阅 :ref:`Add a Link to a Course Unit`.

.. _Export a Course:

***************
输出课程
***************

输出课程的原因如下：

* 保存工作成果
* 直接在课程中编辑可扩展标记语言
* 复制课程，若您之后想将课程改回之前的版本，您可以导入您先前输出的版本
* 与其他教师分享，供上课使用
* 复制课程以便之后导入其他课程并进行客制化 
 
输出课程时，Studio会创建 **.tar.gz** 文档，包括以下课程资料： 
 
* 课程内容（所有章节、小节和单元）
* 课程结构
* 个人问题
* 页面
* 课程优点
* 课程设定

输出的课程资料不包括以下资料：
 
* 用户资料
* 课程小组资料
* 讨论区资料
* 修课证书


#. 从工具栏中选择输出
#. 点击输出课程内容

输出完成后，您就能在电脑上进入tar.gz文档

.. _Import a Course:

***************
 导入课程
***************

.. warning::
	导入的课程会取代之前之前的所有课程内容。导入课程是无法取消的。
	我们建议您首先输出课程内容，做好备份。
 
导入课程的可能原因如下：

* 载入在Studio以外的环境内开发的课程
* 为在Studio以外的环境开发的课程创建新版本

您导入的课程必须是tar.gz格式的文档（文档是经过GNU Zip解压而成的）。
至少必须包含一个 course.xml文档位于课程资料目录。
此tar.gz文档必须与课程资料目录命名相同。目录中可能包含其他文件。
 
如果您的课程使用传统式格式，您可能无法在Studio中编辑课程。
为了保证您的课程完全可编辑，请确保所有的组件都已包含在单元内。
 
导入课程有五个步骤。在前两个步骤中，你必须保留导入界面。
在解压完成后您能离开导入界面。
然而，我们建议您不要对课程进行重大修改，直到导入完成。
 
导入课程：

#. 从工具栏中选择 **导入**
#. 点击选择 **导入文件**
#. 找到您要的文档，然后点击 **打开**
#. 点击 **替代以上我的课程** 

.. note:: 
 当您导入课程时，课程开始时间等重要日期将会被重写。
 导入完成后，您应查看日期以确保其符合您的意愿。详情请参阅： :ref:`Scheduling Your Course`.
 
.. _Work with the targz file:

******************************
.tar.gz文件
******************************

课程将以.tar.gz文件的形式导入和输出。
 
您将需要第三方工具以压缩和解压.tar.gz类型文件。

如果您使用 Microsoft Windows，请参考以下资源：

* `How to Unpack a tar File in Windows
  <http://www.haskell.org/haskellwiki/How_to_unpack_a_tar_file_in_Windows>`_
   
* `How to Extract a Gz File <http://www.wikihow.com/Extract-a-Gz-File>`_
  
* `The gzip Home Page <http://www.gzip.org/>`_

*  在 `Windows <http://www.ofzenandcomputing.com/how-to-open-tar-gz-files/#windows>`_ 
系统下的 `How to Open .tar.gz Files <http://www.ofzenandcomputing.com /how-to-open-tar-gz-files/>`_ 页面。

如果您使用Mac OS X，请参考以下资源：

* 在 `Mac OS X <http://www.ofzenandcomputing.com/how-to-open-tar-gz-
  files/#mac- os-x>`_ 系统下的 `How to Open .tar.gz Files
  <http://www.ofzenandcomputing.com/how-to-open-tar-gz-files/>`_ 页面。

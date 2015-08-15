.. _VitalSource:

#########################
VitalSource 电子阅读器
#########################

VitalSource 书架电子阅读器使你的学生能够轻松访问电子书。除了阅读文档，学生能快速浏览和查找内容（包括图片和笔记），使用多种荧光笔，创建和管理笔记以及复制笔记到外部文档。

.. image:: ../../../shared/building_and_running_chapters/Images/VitalSource.png
   :width: 500
   :alt: VitalSource e-book with highlighted note

想要了解更多关于Vital Source和它的特性，请访问 `VitalSource 书架支持 <https://support.vitalsource.com>`_.

.. note:: 在你添加VitalSource书架电子阅读器到你的课程之前，你必须确保你所需的内容已经存在于Vital Source目录中了。如果内容还不可用，Vital Source与电子书出版商合作来创建电子书以符合VitalSource书架的规格。 **这个过程要花上4个月的时间** 接下来的步骤已假设你想要的电子书已经存在Vital Source目录中。

**************************
添加VitalSource电子阅读器
**************************

添加VitalSource书架电子阅读器有以下几个步骤：

#. :ref:`获取指定信息<VS Obtain VS Info>` 关于你的来自Vital Source的电子书

#. :ref:`修改课程高级设置<VS Modify Advanced Settings>` 使你能够创建一个Vital Source学习工具互操作(LTI)组件

#. :ref:`添加VitalSource书架电子阅读器<VS Add VS EReader>` 到一个单元中

.. _VS Obtain VS Info:

===========================================
步骤一，从VitalSource获取信息
===========================================

要创建一个VitalSource书架电子阅读器，你需要以下来自Vital Source的信息：

-  **LTI 通行证** 》政策密钥，这个密钥使你能为VitalSource书架电子阅读器创建一个LTI组件，更多关于 **LTI 通行证** 政策密钥的信息请参照 :ref:`LTI 信息` 在在 :ref:`LTI 组件`中。

- 你的电子书的重要来源书号（VBID），是Vital Source在添加电子书到它的目录时创建的一个特别码。

要获取这个信息，你的课程团队选择一个成员点成员（MPP）来与Vital Source交互。Vital Source提供了 **LTI 通行证**
政策密钥和VBID给MPP。


.. _VS Modify Advanced Settings:

=============================================
步骤二，修改课程高级设置
=============================================

在这一步骤中，你将要修改课程的高级设置以允许你创建一个LTI组件并添加 **LTI 通行证** 政策密钥。

#. 在Studio中，点击 **设置** 菜单，然后点击 **高级设置**

#. 在  **高级模块列表** 政策密钥域中，把你的光标放置在括号中

#. 输入 ``“lti”``确保包含引号，但没有句号。

   .. image:: ../../../shared/building_and_running_chapters/Images/LTIPolicyKey.png
    :alt: Image of the Advanced Module List key in the Advanced Settings page, with the LTI value added

  .. note:: 如果值域里已经包含文本，直接把光标放在结尾引号后，然后输入一个逗号，后跟 ``“lti”`` （确保你包含了引号） **高级模块列表** 可能类似：

   ``["value_1","lti"]``

4. 向下滚动到 **LTI 通行证** 政策密钥.

#. 在政策值域，把光标放在括号中，然后输入你从Vital Source获取的 **LTI 通行证** 政策密钥的值，确保输入的值用引号标记。

   例如，在这个域中的值与下面类似：

   ``"id_21441:b289378-ctools.school.edu:23746387264"``

6. 在页面的底部，点击 **保存更改**

页面会自动刷新。在页面的顶部，你将看到通知，显示你的更改已经被保存。

.. _VS Add VS EReader:

==============================================================
步骤三，添加VitalSource书架电子阅读器到单元
==============================================================

要添加VitalSource书架电子阅读器到单元，你将创建一个LTI组件，然后在组件中配置几项设置。

#. 在你想在其中创建问题的单元里，点击 **高级**， 在 **添加新的组件**下 然后点击 **LTI**

#. 在出现的组件中，点击 **编辑**

#. 在 **显示名称** 的域中，输入你的电子书的名称，这个名字将在问题上面作为标题出现，并在 **课程件** 页面顶部的学习序列中的作为提示文本

#. 在 **习惯参数** 后点击 **添加**

#. 在出现的域中，输入下列内容（其中 ``VitalSourceCode`` 是电子书的VBID）：

   ``vbid=VitalSourceCode``

   如果你想在课程中用电子书作实验，但你还不想给电子书一个VBID时，你可以输入 ``vbid=L-999-70103`` 来创建一个链接到 *傲慢与偏见*

#. 如果你想电子书打开到特定的一页，再次点击 在**习惯参数** 后面的 **添加** 然后添加下列内容（其中 ``35`` 是电子书中的页码：

   ``book_location=page/35``

#. 在 **启动URL** 域中，输入下列内容（其中用 ``https`` 替代 ``http`` ）：

  ``https://bc.vitalsource.com/books/book``

8. 在 **LTI ID** 域，输入下列内容：

  ``vital_source``

9. 点击 **保存**

**************************
给学生的信息
**************************

第个机构的Vital Source账号管理员将训练MPP如何使用VitalSource书架电子阅读器，并作为过程的的一部分提供支持文档。然而，为了改善学习者的体验，我们建议你把下列的解释提供给你的学生：

  VitalSource书架电子书中的数字课本提供了简单的、用户友好的导航，以及即时的、直观的内容访问。在课程中你将尽可能多地利用以下VitalSource书架电子阅读器特性：

  * 浏览内容，图片，笔记和过滤器搜索结果
  * 运用多种荧光笔
  * 创建和管理笔记
  * 复制和粘贴笔记到外部文档

  关于如何使用这些特性的更多信息，请访问 `VitalSource 书架网址 <https://support.vitalsource.com>`_.


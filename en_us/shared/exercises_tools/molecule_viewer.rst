.. _Molecule Viewer:

#######################
分子浏览器
#######################

系统提供了可以在关于分子讨论中使用两个工具：

* 借助 **分子浏览器** 你可以生成分子的三维模型给学生观看。 
* 借助 **分子编辑器** 的问题模式， 你可以让自己的学生画出自己设计的分子。 有关此工具的更多信息，请参阅 :ref:`Molecule Editor`。

这两个工具都用到了 **JSmol**, 一个由Jmol开发的基于JavaScript的分子浏览器。 (你不需要去下载这个工具，系统会自动使用它。) 有关JSmol的详细信息，请参阅 `JSmol <http://sourceforge.net/projects/jsmol/>`_.

下图显示了在一个课程中的分子浏览器工具：

.. image:: ../../../shared/building_and_running_chapters/Images/MoleculeViewer.png
   :width: 500
   :alt: Image of molecule viewer showing a molecule of Ciprofloxacin



.. note:: 要创建一个分子浏览器，你必须获得将文件上传到第三方文件托管网站的权限，例如 Amazon 的 Web Services Simple Storage Service (AWS S3)。 当你创建了分子浏览器，你会上传一个包含大量文件的文件夹到文件托管网站。 

.. _Create the Molecule Viewer:

*******************************
创建分子浏览器
*******************************

创建分子浏览器需要几个步骤:

#. 从 `BioTopics website <http://www.biotopics.co.uk/jsmol/molecules>`_ 和 edX 上下载所需要的文件。
#. 移动或编辑一些你下载的文件。
#. 上传包含所有你下载并编辑完文件的文件到到你自己的文件托管网站中。
#. 在系统中创建一个包含IFrame的HTML组件。 该IFrame引用你上传到该文件托管网站的文件。

================================================
从 BioTopics 和 edX 上下载软件
================================================

#. 创建或下载你要显示分子的 .mol 文件。 你可以从 `BioTopics website <http://www.biotopics.co.uk/jsmol/molecules>`_ 下载各种 .mol文件。 将文件保存在一个你可以很容易地找到它的地方。
#. 从edX上下载 `MoleculeViewerFiles.zip <http://files.edx.org/MoleculeViewerFiles.zip>`_ 。
#. 解压缩你刚刚下载的 `MoleculeViewerFiles.zip <http://files.edx.org/MoleculeViewerFiles.zip>`_ .

   当你解压缩这个文件时，会看到一个名叫 **MoleculeViewerFiles** 的文件夹，其中包含了一下的文件夹或文件:

    * data (文件夹)
    * j2s (文件夹)
    * js (文件夹)
    * MoleculeViewer.html (文件)

================================================================
移动 .mol 文件并编辑 MoleculeViewer.html 文件
================================================================

#. 将你从 BioTopics 下载的 .mol 文件移动到  into the **data** folder that you downloaded from edX.
#. 编辑 MoleculeViewer.html 文件:

   #. 在文本编辑器中打开MoleculeViewer.html文件。
   #. 在 MoleculeViewer.html 文件中的第19行，用你的 .mol文件名来替换 **Example.mol** 。  例如，你下载了 Glucose.mol 这个文件，那么你文件中的第19行应该是下面的样子:

   		``script: "set antialiasDisplay; background black; load data/Glucose.mol;"``

3. 保存 MoleculeViewer.html 文件。

================================
上传文件到托管网站
================================

#. 确保你的 **MoleculeViewerFiles** 文件夹包含以下的文件夹或文件:

   * data (文件夹): 你已经添加了一个 .mol 文件到该文件夹中。
   * j2s (文件夹)
   * js (文件夹)
   * MoleculeViewer.html (文件): 你已经修改过该文件的第19行。

2. 上传完整的 **MoleculeViewerFiles** 文件夹到你的托管网站上。 

   .. note:: 因为这个文件夹中包含多个文件，即使是快速连接上传文件夹可能也需要几分钟。

===============================
创建一个组件
===============================

#. 打开你想添加组件的位置。
#. 点击 **添加新组件** 中的 **HTML** ，再点击 **IFrame** 。
#. 用自己的文本替换组件编辑器中已有的内容。
#. 点击工具栏中的 **HTML** 。
#. 在 **HTML 源代码** 中，在你想要出现分子浏览器的地方输入以下几行:

   ``<p><iframe name="moleculeiframe" src="https://path_to_folder/MoleculeViewerFiles/MoleculeViewer.html" width="500" height="500"></iframe></p>``

6. 用你文件托管网站的URL来替换 ``path_to_file`` 。 例如下面这行所写的:

   ``<p><iframe name="moleculeiframe" src="https://myfiles.example.com/MoleculeViewerFiles/MoleculeViewer.html" width="500" height="500"></iframe></p>``

7. 点击 **确定** 来关闭 **HTML 源代码** 框，再点击 **保存** 来保存组件。
#. 点击 **预览** 来看你的组件所呈献给学生的效果。

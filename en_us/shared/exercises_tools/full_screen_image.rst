.. _Full Screen Image:

######################
全屏图像工具
######################

有一些较大的图片很难在课程中浏览。全屏图像工具让学生可以放大图片，这样他们就可以看到图片中的详细内容。

****************************************
全屏图像的学生视角
****************************************

学生在单元页面中看到全屏图像。当学生把光标移到图像上时，出现 **全屏** 按钮：

.. image:: ../../../shared/building_and_running_chapters/Images/image-modal.png
 :alt: Image of the full screen image tool with the Full Screen button.

学生点击 **全屏** ，图像将拓展至整个浏览器窗口，出现 **关闭** ，**放大** 和 **缩小** 按钮：

.. image:: ../../../shared/building_and_running_chapters/Images/image-modal-window.png
 :alt: Image of the Image Modal tool with the Full Screen button.

学生可以放大图片，并拖拽以查看图片的不同部分：

.. image:: ../../../shared/building_and_running_chapters/Images/image-modeal-zoomed.png
 :alt: Image of the Image Modal tool with the Full Screen button.

******************************
创建全屏图像
******************************

#. 将图片上传到 **文件与上传** 页面。更多关于如何操作的信息请参阅 :ref:`Add Files to a Course` 。

#. 在 **添加新组件** 下点击 **html** 然后点击 **全屏图像** 。

#. 新组件出现时，点击 **编辑** 。

#.在组件编辑器中，把默认标题替换掉，删掉指导段，并按需要添加文字。

#. 切换到 **HTML** 栏。

#. 将以下占位符替换为您的内容。

   * 将<a>元素href属性的值设为您的图片路径。不要更改class属性的值。例如：

     **<a href="/static/Image1.jpg" class="modal-content">**

   * 将<img>元素的src属性值设为您的图片路径。例如：

     **<img alt="Full screen image" src="/static/Image1.jpg"/>**

   * 确保href和src的属性值相同，且不要更改class属性。您的样本代码应该像下面这样：

   .. code-block:: xml

     <h2>Sample Image Modal</h2>
     <a href="/static/Image1.jpg" class="modal-content">
     <img alt="Full screen image" src="/static/Image1.jpg"/>
     </a>

   .. note:: 您可以在任何HTML组件中使用这样的HTML代码，不仅仅是创建全屏图像时。


#. 点击 **保存** 。

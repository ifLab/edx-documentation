.. _Image Mapped Input:

###########################
《Image Mapped Input Problem》图像映射输入问题
###########################

《In an image mapped input problem, also known as a "pointing on a picture"
problem, students click inside a defined region in an image. You define this
region by including coordinates in the body of the problem.
》在一个图像映射输入问题中，又称图片点击问题，学生在一个图像预定义的区域里点击。你通过在问题本体里面包含坐标来定义这个区域。

.. image:: ../../../shared/building_and_running_chapters/Images/ImageMappedInput-Simple.png
 :width: 500
 :alt: Problem that asks learners to click inside Egypt on a map of Africa

《You can specify the following types of regions.》你可以指定下列区域类型。

* 《One rectangular region. For more information, see》单矩形区域，更多信息请参照 :ref:`《Specify a
  Rectangular Region》指定一个矩形区域`
* 《Multiple rectangular regions. For more information, see》多矩形区域，更多信息请参照 :ref:`《Specify
  Multiple Rectangular Regions》指定多矩形区域`
* 《One non-rectangular region. For more information, see》一个非矩形区域，更多信息请参照 :ref:`《Specify an
  Irregular Region》指定一个不规则区域`

.. note:: 《When you create a problem that contains an image, you must include
 alt text for your image to make the image accessible. For more information
 about alt text, see》当你创建一个包含图像的问题，你必须为你的图像包含alt文本以使图像可访问。关于alt文本的更多信息请参照 :ref:`《Guidelines for Creating Accessible Content》创建可访问内容的指南`

****************************************
《Create an Image Mapped Input Problem》创建一个图像映射输入问题
****************************************

《To create an image mapped input problem, follow these steps.》创建一个图像映射输入问题，遵循下列步骤

#. :ref:`Collect the information that you need for the image<Determine
   Coordinates>`. 

#. :ref:`Create the problem in Studio<Create an IMI Problem in Studio>`.

.. _Determine Coordinates:

============================
《Collect Image Information》收集图像信息
============================

《To create an image mapped input problem, you need the following elements.》创建一个图像映射输入问题，你需要下列元素

   * 《The height and width of the image in pixels.》图像的高度和宽度，单位pixel
   * 《Coordinate pairs that define the region or regions where you want
     students to click.》定义区域的坐标对或你想让学生点击的区域

《To collect the information you need about your image, use an image editing
tool such as Microsoft Paint.》收集你需要的关于图像的信息，用一个图像编辑工具，比如Microsoft Paint.

.. note:: 《The coordinate pairs for all images start with (0,0) in the
 upper-left corner of the image and increase in value toward the lower-right
 corner, similar to the progression of reading English.
》所有图像的坐标对在左上角以(0,0)开始，然后往右下方增加，与读英语的前进方向类似。

* 《To specify a rectangular region, you need two coordinate pairs: the
  upper-left corner and the lower-right corner.》指定一个矩形区域，你需要两个坐标对：左上角和右下角

* 《To specify more than one rectangle, you need the coordinate pairs for the
  upper-left and lower-right corners of each rectangle.》指定多个矩形，你需要每个矩形的左上角和右下角的坐标对

* 《To specify an irregular region, you need three or more coordinate pairs.
  Studio creates the simplest possible shape based on these coordinate
  pairs. You can enter the coordinate pairs in any order.
》指定一个不规则的区域，你需要三个或更多的坐标对。Studio创建基于三个坐标对的最简单的形状

  《For example, for a triangle, you need three coordinate pairs. For an
  octagon, you need eight coordinate pairs.》例如，对于一个三角形，你需要三个坐标对，对于一个八边形，你需要八个坐标对。

.. _Create an IMI Problem in Studio:

=================================
《Create the Problem in Studio》在Studio中创建问题
=================================

#. 《In Studio, upload your image to the》在Studio中，上传你的图像到 **《Files & Uploads》文件和上传** 《page, and make a
   note of the file path for the image. For more information, see》页面，并给图像的文件路径做注释。更多信息请参照 :ref:`《Add
   Files to a Course》添加文件到课程`
#. 《In the unit where you want to create the problem, click》在你想创建问题的单元中，点击 **《Problem》问题** 《
   under》在 **《Add New Component》添加新的组件** 《, and then click the》下，点击 **《Advanced》高级** 《tab.》图标
#. 《Click》点击 **《Image Mapped Input》图像映射输入**
#. 《In the component that appears, click》在出现的组件中，点击 **《Edit》编辑**
#. 《In the component editor, replace the example problem text with your own text.》在组件编辑器中，用你自己的文本替换示例问题。
#. 《In the》在 ``<imageinput>`` 《element, follow these steps.》元素中，遵循下列步骤

   #. 《Replace the example file path in the》在 ``《src》源`` 《attribute with the file
      path for your image.》属性中用你的图像的路径替换示例文件路径

   #. 《Include alt text for your image to make the image accessible. For more
      information about alt text, see》包含alt文本使得你的图像可访问。更多关于alt文本的信息请参照 :ref:`《Guidelines for Creating Accessible
      Content》创建可访问内容的指南`

   #. 《Replace the example values for the》用你的图像的尺寸替换示例中的 ``《width》宽度`` 《and》和 ``《height》高度`` 《attributes
      with the dimensions for your image.》属性值

   #. 《Modify the example》修改示例 ``《rectangle》矩形`` 《attribute to reflect the shape and size
      of the region that you want to specify. For more information, see》的属性来反映你想指定的区域的形状和尺寸。更多信息请参照
      :ref:`《Specify a Rectangular Region》指定一个矩形区域`， :ref:`《Specify Multiple Rectangular
      Regions》指定多个矩形区域`《, or》，或 :ref:`《Specify an Irregular Region》指定一个不规则区域`

#. 《Click》点击 **《Save》保存**

.. _Specify a Rectangular Region:

《Specify a Rectangular Region》指定一个矩形区域
****************************************

《To specify a rectangular region, edit the》指定一个矩形区域，编辑 ``《rectangle》矩形`` 《attribute in the》属性，在
``<imageinput>`` 《element.》元素中

* 《Specify the coordinate pair for the upper-left and lower-right corners of
  the rectangle, separating the x and y values with a comma.》指定矩形的左上角和右下角的坐标对，用逗号分隔x和y坐标值
* 《Surround each coordinate pair with parentheses.》用圆括号包围坐标对
* 《Use a hyphen to separate the coordinate pairs.》用连字号分隔坐标对
* 《Surround the set of coordinate pairs with quotation marks》用双引号 (")包围多个坐标对


《For example, the following》例如，接下来的 ``《rectangle》矩形`` 《attribute creates one rectangle from
two coordinate pairs:》属性以两个坐标对创建一个矩形：

``rectangle="(338,98)-(412,168)"``

**《Problem Code》问题代码**:

.. code-block:: xml

 <problem> 

  <p>What country is home to the Pyramids as well as the cities of
  Cairo and Memphis? Click the country on the map below.</p> 

  <imageresponse>
    <imageinput src="/static/Africa.png" width="600" height="638"
  rectangle="(338,98)-(412,168)" alt="Map of Africa" />
  </imageresponse>
 
  <solution> 
    <div class="detailed-solution"> 
  
      <p>Explanation</p> 
  
      <p>Egypt is home to not only the Pyramids, Cairo, and Memphis, but also the
  Sphinx and the ancient Royal Library of Alexandria.</p>
  
    </div> 
  </solution> 

 </problem>

.. _Specify Multiple Rectangular Regions:

《Specify Multiple Rectangular Regions》指定多个矩形区域
****************************************

《You can specify more than one rectangular region in an image.》你可以在一个图像中指定多个矩形区域

.. image:: ../../../shared/building_and_running_chapters/Images/ImgMapInput_Mult.png
 :width: 350
 :alt: Problem that asks students to click inside one of three rectangles

《To specify multiple rectangular regions, edit the》指定多个矩形区域，编辑 ``《rectangle》矩形`` 《attribute in the
》属性，在``<imageinput>`` 《element.》属性中

* 《Specify the coordinate pair for the upper-left and lower-right corners of
  each rectangle, separating the x and y values with a comma.》指定矩形的左上角和右下角的坐标对，用逗号分隔x和y坐标值
* 《Surround each coordinate pair with parentheses.》用圆括号包围坐标对
* 《Use a hyphen (-) to separate the coordinate pairs.》用连字号(-)分隔坐标对
* 《Separate each rectangle with a semicolon》用分号(;)分隔每个矩形
* 《Surround the entire set of coordinates with quotation marks》用双引号(")包围整个坐标集

《For example, the following》例如，接下来的 ``《rectangle》矩形`` 《attribute creates three rectangles:》属性创建三个矩形：

``rectangle="(62,94)-(262,137);(306,41)-(389,173);(89,211)-(187,410)"``

**《Problem Code》问题代码**:

.. code-block:: xml

 <problem>
  
  <p>In the following image, click inside any of the rectangles.</p>
    
    <imageresponse> 

      <imageinput src="/static/imageresponse_multipleregions.png" width="450"
        height="450" rectangle="(62,94)-(262,137);(306,41)-(389,173);(89,211)-
        (187,410)" alt="Three rectangles on a white background" />
        
    </imageresponse>
    
 </problem>

.. _Specify an Irregular Region:

《Specify an Irregular Region》指定一个非规则区域
****************************************

《You can specify one non-rectangular region.》你可以指定一个非矩形区域

.. image:: ../../../shared/building_and_running_chapters/Images/ImgMapInput_Irreg.png
  :width: 500
  :alt: Problem that asks learners to click inside a pentagon

《To specify an irregular region, edit the》指定一个非规则区域，编辑 ``《rectangle》矩形`` 《attribute in the
》属性，在 ``<imageinput>`` 《element.》元素中

* 《Change》更改 ``《rectangle》矩形`` 《to》成 ``《region》区域``
* 《Specify three or more coordinate points in any order.》以做任意顺序指定三个或更多坐标点
* 《Enter each coordinate pair in brackets》在中括号 ([])中输入每个坐标对 **《Do not use parentheses》不要用圆括号**
* 《Separate each set of points with a comma》用逗号 (,) 《and a space.》和空格来分隔每个点集
* 《Enclose the whole list of coordinate points in brackets》有中括号 ([])把全部坐标点包围起来
* 《Surround the outer brackets with quotation marks》用双引号(")把外部的中括号包围起来

《For example, the following》例如，接下来的 ``《regions》区域`` 《attribute creates a pentagon.》属性创建一个五边形

``regions="[[219,86], [305,192], [305,381], [139,381], [139,192]]"``

**《Problem Code》问题代码**:

.. code-block:: xml

 <problem>

  <p>In the following image, click inside the pentagon.</p>
  
  <imageresponse> 

    <imageinput src="/static/imageresponse_irregularregions.jpg" width="600"
    height="204" regions="[[219,86], [305,192], [305,381], [139,381],
    [139,192]]" alt ="A series of 10 shapes including a circle, triangle,
    trapezoid, pentagon, star, and octagon" />

  </imageresponse>

 </problem>

.. _Image Mapped Input Problem XML:

******************************
《Image Mapped Input Problem XML》图像映射输入问题XML
******************************

==========
《Template》模板
==========

.. code-block:: xml

  <problem>

    <p>Problem text</p>

        <imageresponse>

         <imageinput src="IMAGE FILE PATH" width="NUMBER" height="NUMBER"
         rectangle="(X-AXIS,Y-AXIS)-(X-AXIS,Y-AXIS)" alt="DESCRIPTION OF
         IMAGE" />

        </imageresponse>

  </problem>

=====
《Tags》标签
=====

* ``<imageresponse>``: 《Indicates that the problem is an image mapped input problem.》表明问题是一个图像映射输入问题
* ``<imageinput>``: 《Specifies the image file and the region in the file that the student must click.》指定图像文件和文件里学生必须点击的的区域。

**《Tag:》标签：** ``<imageresponse>``

《Indicates that the problem is an image mapped input problem.》表明问题是一个图像映射输入问题

  《Attributes》属性

  《(none)》（空）

  《Children》子标签

  * ``<imageinput>``

**《Tag:》标签：** ``<imageinput>``

《Specifies the image file and the region in the file where students must click.》指定图像文件和文件里学生必须点击的的区域。

  《Attributes》属性

   .. list-table::
      :widths: 20 80

      * - 《Attribute》属性
        - 《Description》描述
      * - ``《src》源`` 《(required)》（必需）
        - 《The URL of the image》图像的URL
      * - ``《height》高度`` 《(required)》（必需）
        - 《The height of the image, in pixels》图像的高度，单位pixel
      * - ``《width》宽度`` 《(required)》（必需）
        - 《The width of the image, in pixels》图像的宽度，单位pixel
      * - ``《rectangle》矩形`` 《(required) (or, for irregular regions》（必需），（或者，对不规则区域区域 ``region``）
        - 《An attribute with two or more coordinate pairs that define the region
          where students should click》有两个或更多坐标对的属性，定义了学生应该点击的区域
      * - ``alt`` 《(required)》（必需）
        - 《A description of the image, used for accessibility》图像的描述，用于可访问性。

  《Children》子标签
  
  《(none)》（空）


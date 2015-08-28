.. _Drag and Drop:

##########################
拖放问题
##########################

在拖放的问题中，学生通过拖动文本或对象到图像的特定位置上来对问题作出回答。

.. image:: ../../../shared/building_and_running_chapters/Images/DragAndDropProblem.png
 :alt: Image of a drag and drop problem

*********************************
创建一个拖放问题
*********************************

要创建一个简单的拖放问题，让学生拖动标签到图像，你需要上传一个图片来让学生在其上拖动标签，之后再创建问题组件。

#. 在 **文件和上传** 页面, 上传你的图片文件。 有关上传文件的详细信息，请参阅 :ref:`Add Files to a Course` 。
#. 在您要创建问题的单元，点击 **添加新的组件** 中的 **问题** , 然后再点击 **高级** 选项卡。
#. 点击 **拖放** 。
#. 点击出现组件中的 **编辑** 。
#. 用你自己的文本替换组件编辑器中的样例文本。
#. 用你上传到 **文件和上传** 页面图片的URL来替换``<drag_and_drop_input>`` 标记中的 **https://studio.edx.org/c4x/edX/DemoX/asset/L9_buckets.png** (例如： **/static/Image.png**)。
#. 对至少一个 ``<draggable>`` 标记，用你希望学生拖动标签中的文字内容来替换 **label** 属性的中的文本。 例如，如果你想让学生单词“Iceland”拖放到您图像上，则新的标签将类似于以下内容：
   
   ``<draggable id="1" label="Iceland"/>``

8. 重复上一步直到你设置完了所有需要的标签。 确保每一个``<draggable>`` 标记的 **id** 属性的值都是不同的。
#. 确定图像上的正确区域的坐标和半径。
#. 在 ``correct_answer = {``中, 以下面的格式为每个标签添加条目。 这些值以像素为单位：

    ``'id':    [[x coordinate, y coordinate], radius]``

    例如,如果你的图片是600像素宽，400像素高， 你希望你的学生到冰岛的标签拖动到一个区域在图像的左上部分，拖动一个瑞典标签靠近图像的右下角部分，该代码将类似于以下 (其中2是瑞典标签的ID):

    .. code-block:: xml

        correct-answer = {
                '1':    [[50, 50], 75]
                '2':    [[550, 350], 75]}

    .. note:: 确保代码包含右大括号 (**}**) 。 
#. 点击 **保存** 。

==========================================
简单拖放问题的代码
==========================================

要创建出现上面图片中的拖放问题，你需要从edX上下载两个文件，并将这些文件上传到 **文件和上传** 的页面中, 然后添加这个问题的代码到一个问题组件中去。

#. 从 edX 上下载这些文件:

  * Allopurinol.gif
  * AllopurinolAnswer.gif

  点击 http://files.edx.org/DragAndDropProblemFiles.zip 下载包含这两个文件的压缩包。

2. 上传 Allopurinol.gif 和 AllopurinolAnswer.gif 这两个文件到 **文件和上传** 页面。
#. 在你想要添加问题的位置，点击 **添加新的组件** 中的 **问题**  然后再点击 **高级** 选项卡 。
#. 点击 **拖放** 。
#. 点击出现组件中的 **编辑** 。
#. 在组件编辑器中用下面的代码替换示例代码。
#. 点击 **保存** 。

**问题的代码**:

.. code-block:: xml

  <problem>
    <p> Allopurinol is a drug used to treat and prevent gout, a very painful form of arthritis. Once only a “rich man’s disease”, gout has become more and more common in recent decades – affecting about 3 million people in the United States alone. Deposits of needle-like crystals of uric acid in connective tissue or joint spaces cause the symptoms of swelling, stiffness and intense pain. Individuals with gout overproduce uric acid because they cannot eliminate it efficiently. Allopurinol treats and prevents gout by stopping the overproduction of uric acid through inhibition of an enzyme required for the synthesis of uric acid. </p>
    <p> You are shown one of many possible molecules. On the structure of allopurinol below, identify the functional groups that are present by dragging the functional group name listed onto the appropriate target boxes on the structure. If you want to change an answer, you have to drag off the name as well. You may need to scroll through the names of functional groups to see all options. </p>
    <customresponse>
      <drag_and_drop_input no_labels="true" one_per_target="true" target_outline="true" img="/static/Allopurinol.gif">
        <draggable can_reuse="true" label="methyl" id="1"/>
        <draggable can_reuse="true" label="hydroxyl" id="2"/>
        <draggable can_reuse="true" label="amino" id="3"/>
        <draggable can_reuse="true" label="carboxyl" id="4"/>
        <draggable can_reuse="true" label="aldehyde" id="5"/>
        <draggable can_reuse="true" label="phosphate" id="6"/>
        <draggable can_reuse="true" label="sulfhydryl" id="7"/>
        <draggable can_reuse="true" label="phenyl" id="8"/>
        <draggable can_reuse="true" label="none" id="none"/>
        <target id="0" h="53" w="66" y="55.100006103515625" x="131.5"/>
        <target id="1" h="113" w="55" y="140.10000610351562" x="181.5"/>
      </drag_and_drop_input>
      <answer type="loncapa/python"> 
  correct_answer = [ {'draggables': ['2'], 'targets': ['0' ], 'rule':'unordered_equal' }, 
  {'draggables': ['none'], 'targets': ['1' ], 'rule':'unordered_equal' }] 
  if draganddrop.grade(submission[0], correct_answer): 
      correct = ['correct'] 
  else: 
      correct = ['incorrect'] 
      </answer>
    </customresponse>
    <solution>
      <img src="/static/AllopurinolAnswer.gif"/>
    </solution>
  </problem>


.. _Drag and Drop Problem XML:

*********************************
拖放问题的XML
*********************************

.. code-block:: xml

    <problem>
        Here's an example of a "Drag and Drop" question set. Click and drag each word in the scrollbar below, up to the numbered bucket which matches the number of letters in the word.
        <customresponse>
            <drag_and_drop_input img="https://studio.edx.org/c4x/edX/DemoX/asset/L9_buckets.png">
                <draggable id="1" label="a"/>
                <draggable id="2" label="cat"/>
                <draggable id="3" label="there"/>
                <draggable id="4" label="pear"/>
                <draggable id="5" label="kitty"/>
                <draggable id="6" label="in"/>
                <draggable id="7" label="them"/>
                <draggable id="8" label="za"/>
                <draggable id="9" label="dog"/>
                <draggable id="10" label="slate"/>
                <draggable id="11" label="few"/>
            </drag_and_drop_input>
            <answer type="loncapa/python">
               correct_answer = {
                   '1':      [[70, 150], 121],
                   '6':      [[190, 150], 121],
                   '8':      [[190, 150], 121],
                   '2':      [[310, 150], 121],
                   '9':      [[310, 150], 121],
                   '11':     [[310, 150], 121],
                   '4':      [[420, 150], 121],
                   '7':      [[420, 150], 121],
                   '3':      [[550, 150], 121],
                   '5':      [[550, 150], 121],
                   '10':     [[550, 150], 121]}
                   if draganddrop.grade(submission[0], correct_answer):
                       correct = ['correct']
                   else:
                       correct = ['incorrect']
            </answer>
        </customresponse>
        <customresponse>
            <text>
                <h2>Drag and Drop with Outline</h2>
                <p>Please label hydrogen  atoms connected with left carbon atom.</p>
            </text>
            <drag_and_drop_input img="https://studio.edx.org/c4x/edX/DemoX/asset/ethglycol.jpg" target_outline="true" one_per_target="true" no_labels="true" label_bg_color="rgb(222, 139, 238)">
                <draggable id="1" label="Hydrogen" />
                <draggable id="2" label="Hydrogen" />
                <target id="t1_o" x="10" y="67" w="100" h="100"/>
                <target id="t2" x="133" y="3" w="70" h="70"/>
                <target id="t3" x="2" y="384" w="70" h="70"/>
                <target id="t4" x="95" y="386" w="70" h="70"/>
                <target id="t5_c" x="94" y="293" w="91" h="91"/>
                <target id="t6_c" x="328" y="294" w="91" h="91"/>
                <target id="t7" x="393" y="463" w="70" h="70"/>
                <target id="t8" x="344" y="214" w="70" h="70"/>
                <target id="t9_o" x="445" y="162" w="100" h="100"/>
                <target id="t10" x="591" y="132" w="70" h="70"/>
            </drag_and_drop_input>
            <answer type="loncapa/python">
                correct_answer = [{
                    'draggables': ['1', '2'],
                    'targets': ['t2', 't3', 't4' ],
                    'rule':'anyof'
                }]
                if draganddrop.grade(submission[0], correct_answer):
                    correct = ['correct']
                else:
                    correct = ['incorrect']
            </answer>
        </customresponse>
    </problem>


========
标记
========

* ``<customresponse>``: 表示该问题是一个自定义回答问题。

* ``<drag_and_drop_input>``: 表示自定义回答问题是一个拖放问题。

* ``<draggable>``: 指定学生将拖到基础图像中的一个对象。

* ``<target>``: 指定拖拽元素在基本图片上所要放置的位置。

**标记:** ``<drag_and_drop_input>``

  属性

  .. list-table::
     :widths: 20 80
     :header-rows: 1

     * - 属性
       - 说明
     * - img (必要的)
       - 将成为基本图像的图片的相对路径。 所有的拖拽元素可以拖动到它。
     * - target_outline 
       - 指定 目标周围 (如果指定了它们) 是否画出轮廓线 (灰色虚线)。 它的值可以是'true' 或者 'false'。
         如果没有指定则目标没有轮廓线。
     * - one_per_target 
       - 指定是否允许多余于一个拖拽元素被放置在同一个目标中。 的值可以是'true' 或者 'false'。
         如果没有指定，默认值是 'true'.
     * - no_labels (必要的)
       - 默认值是 false 。 默认行为中，如果标签没有设置，标签从ID获得。 如果 no_labels 设置为 true ，那么标签不会自动由ID生成，一个不能设置标签，将获得唯一的图标。

  子标记

     * ``<draggable>``
     * ``<target>``

**标记:** ``<draggable>``

指定拖放问题中的一个拖拽元素。

拖拽元素是用户必须拖出滑块并拖放到基本图像上。 完成拖动操作后，如果拖拽元素的中心位于图像矩形区域之外，它将被退回滑块中去。

为了便于评分，每个拖拽元素都要有唯一的ID。

  属性

  .. list-table::
     :widths: 20 80
     :header-rows: 1

     * - 属性
       - 说明
     * - id (必须的)
       - 拖拽元素唯一的标识。
     * - label (可选的)
       - 用户可以看到的文本标签。
     * - icon (可选的)
       - 当拖拽元素是图片时，图片文件的相对路径。
     * - can_reuse
       - 默认情况下为false。 如果设置为true，则同一个拖拽元素可以使用多次。

  子标记
  
  (无)

**标记:** ``<target>``

指定基本图片上学生必须放置拖拽元素的位置。 按照设计如果拖拽元素的中心在目标区域之内，即在由 [[x, y], [x + w, y + h]] 所指定的矩形区域内，则该元素在目标区域内。
否则就在目标区域之外。

如果你至少指定了一个目标，当学生将拖拽元素拖放到目标之外时，拖拽元素会被退回到滑块中。

如果你没有指定目标区域，学生可以把拖拽元素放到基本图片上的任何位置。

  属性

  .. list-table::
     :widths: 20 80
     :header-rows: 1

     * - 属性
       - 说明
     * - id (必须的)
       - 拖拽元素唯一的标识。
     * - x
       - 目标区域的左上角将定位在基本图像上的X坐标。
     * - y
       - 目标区域的左上角将定位在基本图像上的Y坐标。
     * - w
       - 目标区域的宽度，以像素为单位。
     * - h
       - 目标区域的高度，以像素为单位。

  子标记

  (无)

**********************
拖拽元素目标
**********************

有时只把基本图片作为目标是不够的，所有的拖拽元素也可以成为目标。 在一个复杂问题中，其中一个拖拽元素本身必须成为一个目标（或者多个目标），则可以使用下面的扩展语法。

::

    ...
    <draggable {attribute list}>
        <target {attribute list} />
        <target {attribute list} />
        <target {attribute list} />
        ...
    </draggable>
    ...

上面标记中的 (``draggable`` and ``target``) 属性和正常的 ``draggable`` and ``target`` 标记是一样的。 唯一的区别是你指定内部目标位置坐标的方法。 用 ``x`` 和
``y`` 属性来设定内部目标到父元素左上角的偏移量 (包含内部目标)。

=====================================
拖拽元素目标的限制
=====================================

* 目前有目标嵌套层数的限制。

  即使你可以在拖拽元素上堆放大量的拖拽元素目标， 拖放问题也只能最多识别两层嵌套的目标。 第一层是 `基础` 目标。 他们在基础图片上。 第二层是定义在拖拽元素上的目标。

* 另一个限制是，在目标范围不针对其他目标检查。

  你必须确保有目标没有重叠。 你也应该确保拖拽元素目标比它的父拖动元素大小要小。 技术上，这是没有必要的，但是从可用性的角度看，它是有必要的。

* 只有定义了基本目标，你猜可以定义拖拽元素目标 ( 基础目标在基础图片上) 。

  如果你没有基础的目标，那么你只能有嵌套一个级别 (基础图片上的拖拽元素)。 在这种情况下，客户端将报告每个拖拽元素在基本图像上位置的坐标（X，Y）。

**********************
正确答案格式
**********************

为目标的拖拽元素指定答案，请参阅 `Answer format for
targets on draggables`_.

有两种正确答案的格式：详细形式和简短形式。

简短形式的正确答案是 ``draggable_id`` 到 ``target_id``的映射::

    correct_answer = {'grass':     [[300, 200], 200], 'ant': [[500, 0], 200]}
    correct_answer = {'name4': 't1', '7': 't2'}

详细形式的答案是一个字典列表。 每个字典有三个要素：
``拖拽元素``, ``目标`` and ``规则`` 。 例如::

    correct_answer = [
    {
      'draggables':   ['7', '8'],
      'targets':  ['t5_c', 't6_c'],
      'rule': 'anyof'
    },
    {
      'draggables': ['1', '2'],
      'targets': ['t2_h', 't3_h', 't4_h', 't7_h', 't8_h', 't10_h'],
      'rule': 'anyof'
    }]

"拖拽元素" 是拖拽元素ID的列表。 "目标" 是ID列表中的拖拽元素所要被放置的位置。

.. 注意::
   ``正确答案`` 列表中的拖拽元素不能相同。

错误 (因为拖拽元素的id 7重复了)::

    correct_answer = [
    {
      'draggables':   ['7', '8'],
      'targets':  ['t5_c', 't6_c'],
      'rule': 'anyof'
    },
    {
      'draggables': ['7', '2'],
      'targets': ['t2_h', 't3_h', 't4_h', 't7_h', 't8_h', 't10_h'],
      'rule': 'anyof'
    }]

 ``规则`` 值如下。

* ``准确``:  ``用户答案`` 的拖拽元素对应的目标，必须和正确答案的相同。 例如，如果 ``正确答案`` 设置如下，那么对于拖拽元素7和8，用户必须将拖拽元素7拖到目标1，将拖拽元素8拖到目标2::

    correct_answer = [
      {
      'draggables':   ['7', '8'],
      'targets':  ['tartget1', 'target2'],
      'rule': 'exact'
    }]


* ``无序``: 允许拖拽元素不按顺序被拖放到目标中。 如果学生要把拖拽元素7和8分别放到目标1,2中，且7,8必须放在不同的目标中，那么正确答案为::

    correct_answer = [
    {
      'draggables':   ['7', '8'],
      'targets':  ['tartget1', 'target2'],
      'rule': 'unordered_equal'
    }]


* ``任意``: 允许拖拽元素被放置任意目标处。 在 `任意` 规则下，学生把拖拽元素7和8拖到目标1或2中的任意一个均正确::

    correct_answer = [
    {
      'draggables':   ['7', '8'],
      'targets':  ['tartget1', 'target2'],
      'rule': 'anyof'
    }]

如果 ``可重用`` 为true， 你有拖拽元素a,b,c和10个目标。 这时你可以将4个拖拽元素 ``a`` 放置到 [``目标1``,  ``目标4``, ``目标7``, ``目标10``]； 而不用重复地写四个 ``a`` 。 这也允许你将拖拽元素 ``b``拖动到目标2和目标5，或者目标5和目标2::

    correct_answer = [
        {
          'draggables': ['a'],
          'targets': ['target1',  'target4', 'target7', 'target10'],
          'rule': 'unordered_equal'
        },
        {
          'draggables': ['b'],
          'targets': ['target2', 'target5', 'target8'],
          'rule': 'anyof'
        },
        {
          'draggables': ['c'],
          'targets': ['target3', 'target6', 'target9'],
          'rule': 'unordered_equal'
        }]

有时你只想让学生移动两个 ``b`` 拖拽元素。 在这种情况下你要使用 ``任意和数字`` 或者 ``无序和数字`` 规则::

    correct_answer = [
        {
          'draggables': ['a', 'a', 'a'],
          'targets': ['target1',  'target4', 'target7'],
          'rule': 'unordered_equal+number'
        },
        {
          'draggables': ['b', 'b'],
          'targets': ['target2', 'target5', 'target8'],
          'rule': 'anyof+number'
        },
        {
          'draggables': ['c'],
          'targets': ['target3', 'target6', 'target9'],
          'rule': 'unordered_equal'
        }]

当每个目标没有多重拖拽元素 (one_per_target=``true``)，
对相同的拖拽元素数， ``任意`` 和 ``无序`` 是等价的。

如果 ``can_reuse=true``,你必须使用详细形式的正确答案。

=======================================
拖拽元素目标的答案格式
=======================================

在上述的情况下， 答案必须提供每个拖拽元素的精确定位。 (对必须驻留的目标)。 当拖拽元素需要被拖放到本身也是拖放元素的目标上时，答案必须包括 目标-拖拽元素-目标 链。

例如，假设我们有三个拖拽元素 - ``up``, ``s``, 和 ``p``。
拖拽元素 ``s`` 和 ``p`` 还是目标。 更具体的， ``p`` 有三个目标 - ``1``, ``2``, 和 ``3``。 第一个要求是 ``s`` 和 ``p`` 被正确放置在基础图片上的指定位置。 第二个要求是拖拽元素 ``up`` 被放在指定的目标 ``p`` 上。  下面是一个问题的节选::

    <draggable id="up" icon="/static/images/images_list/lcao-mo/up.png" can_reuse="true" />

    <draggable id="s" icon="/static/images/images_list/lcao-mo/orbital_single.png" label="s orbital" can_reuse="true" >
        <target id="1" x="0" y="0" w="32" h="32"/>
    </draggable>

    <draggable id="p" icon="/static/images/images_list/lcao-mo/orbital_triple.png" can_reuse="true" label="p orbital" >
      <target id="1" x="0" y="0" w="32" h="32"/>
      <target id="2" x="34" y="0" w="32" h="32"/>
      <target id="3" x="68" y="0" w="32" h="32"/>
    </draggable>

    ...

    correct_answer = [
        {
          'draggables': ['p'],
          'targets': ['p-left-target', 'p-right-target'],
          'rule': 'unordered_equal'
        },
        {
          'draggables': ['s'],
          'targets': ['s-left-target', 's-right-target'],
          'rule': 'unordered_equal'
        },
        {
          'draggables': ['up'],
          'targets': ['p-left-target[p][1]', 'p-left-target[p][2]', 'p-right-
             target[p][2]', 'p-right-target[p][3]',],
          'rule': 'unordered_equal'
        }
    ]

注意！你必须为每一个拖拽元素指定规则，即使有拖拽元素包含在多个链中。

*************
评分逻辑
*************

#. 学生的答案和正确答案有着几乎相同的格式。
   ::

    group_id: group_draggables, group_targets, group_rule

  ``group_id`` 是序数，用来记录每个正确答案中字典的增量。
  ``group_id`` 是被分配: 0, 1, 2, ...

  用户答案中的拖拽元素被添加到和正确答案中的拖拽元素具有相同group_id的组中，例如::

    如果正确答案拖拽元素组[group_0] = [t1, t2] 那么用户拖拽元素组[group_0]就是用户答案中所有的拖拽元素 t1 和 t2 :
    [t1] or [t1, t2] or [t1, t2, t2] etc..

2. 对于每个用户答案组中的拖拽元素， 如果 ``数字`` 在组的规则中， 那么set()会被应用。 如果 ``数字`` 不在规则中，则不会被应用::

    set() : [t1, t2, t3, t3] -> [t1, t2, ,t3]

  对于每一个组，在这个步，拖拽元素列表是相等的。

3. 对于每一个组，目标列表是使用该组的规则进行比较。

==========================
``set()`` 和 ``数字`` 事件
==========================

``set()`` and ``+number`` 仅用于有可重复使用的拖拽元素的情况。
其他情况下，有在列表中没有相等的拖拽元素，所以 set() 什么效果都没有。

*  ``set()`` 操作允许你创造一个规则来规定 "任何数量相同的拖拽元素可以拖动到目标"::

    {
      'draggables': ['draggable_1'],
      'targets': ['target3', 'target6', 'target9'],
      'rule': 'anyof'
    }

* ``数字`` 规则被用于有可重复使用的拖拽元素的情况中，来修复修复拖动的拖动元素数量。 在本实施例只有两个实例draggables_1的允许被拖动::

    {
      'draggables': ['draggable_1', 'draggable_1'],
      'targets': ['target3', 'target6', 'target9'],
      'rule': 'anyof+number'
    }


* 注意！ 在使用 ``准确``规则的情况下，是不需要 ``数字``规则的。 因为你不能从用户界面识别可重复使用的拖拽元素是哪个目标的。 例如::

    {
      'draggables': ['draggable_1', 'draggable_1', 'draggable_2'],
      'targets': ['target3', 'target6', 'target9'],
      'rule': 'exact'
    }


    本实例的正确处理是分别对 draggable_1 和 draggable_2 创建不同的规则。

* 对于 ``无序`` (或者 ``准确``) 你不需要 ``数字``。 如果你只有相同的拖拽元素在组中，目标长度将提供对拖拽元素数量的约束::

    {
      'draggables': ['draggable_1'],
      'targets': ['target3', 'target6', 'target9'],
      'rule': 'unordered_equal'
    }

  这意味着仅有 ``draggable_1`` 可以被拖拽。

* 但是，如果你有多个不同的可重复使用的拖拽元素在列表中，你可以使用``number``规则::

    {
      'draggables': ['draggable_1', 'draggable_1', 'draggable_2'],
      'targets': ['target3', 'target6', 'target9'],
      'rule': 'unordered_equal+number'
    }

如果你没有使用 ``数字``， 那么拖拽元素列表会被设置成[``draggable_1``, ``draggable_2``]。

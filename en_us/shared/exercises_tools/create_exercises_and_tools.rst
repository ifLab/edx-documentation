.. _Create Exercises:

############################
创建练习和工具
############################

************************************
练习和工具的说明
************************************

Studio允许你为你的课程创建多种多样的练习和工具.其中有很多的练习和工具在Studio有模板帮助你创建练习. 另外, 个别的课程团队经常创建在Studio没有的练习. 

.. note::edX提供给每个不同工具的支持程度是不同的.不完全由edX提供支持的练习和工具会被用临时或不支持的指标标记.

   暂时性支持的练习和工具可能会缺少你使用edX建立课程功能的稳定性。不被edX支持的练习和工具不被edX保持，将来可能会被弃用。


   根据练习和工具, 你使用 HTML, 问题,或者高级组件. 每个人的练习或工具页面都包含一个练习或工具的例子，连同所有文件，代码，和一步步的说明。

.. note:: 当你创建问题时你必须包含可访问的标签。可访问的标签通常包含你的主要问题文本。标签的说明会出现在每个人问题的页面中。

****************************
一般的练习和工具
****************************

.. list-table::
   :widths: 30 25 60 20

   * - .. image:: ../../../shared/building_and_running_chapters/Images/AnnotationExample.png
          :width: 100
          :alt: 注释问题示例
     - :ref:`注释`
     - 注释问题让学生回答一个特殊的文本区域.这个问题出现在文本上方当学生将光标移动到高亮文本时，这能让学生思考在阅读时能这个问题。
     - 暂时支持
   * - .. image:: ../../../shared/building_and_running_chapters/Images/PollExample.png
          :width: 100
          :alt: 调查示例
     - :ref:`条件模块`
     -  你可以创建一个条件模板去控制学生可以看到的内容版本.比如，对于一个调查问题回答Yes的学生然后从对这个问题回答No学生看到一块不同的文本.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/JavaScriptInputExample.png
          :width: 100
          :alt: Example JavaScript problem
     - :ref:`自定义JavaScript`
     - 自定义JavaScript显示和评分问题(也叫*自定义JavaScript问题* or *JS输入问题*)允许你创建一个
       自定义问题或工具使用JavaScript然后吧这个问题或工具直接添加到Studio.
     - 完全支持   
   * - .. image:: ../../../shared/building_and_running_chapters/Images/external-grader-correct.png
          :width: 100
          :alt: Example external grader
     - :ref:`External Grader`
     - external grader是一个接受并处理学生对一个问题的回答的服务,然后把这些问题回馈返回到edX平台上.你可以从edX平台上单独创建并配置一个external grader.external           grader对于处理软件编程课程中学生提交的复杂的代码非常有用.
     - 暂时支持 
   * - .. image:: ../../../shared/building_and_running_chapters/Images/google-calendar.png   
          :width: 100
          :alt:谷歌日历
     - :ref:`谷歌日历工具`
     - 你可以在你的课程中嵌入谷歌日历以便学生能在你的课件中看到这个日历.你可以使用谷歌日历分享测试日期, 办公时间或其他学生感兴趣的日程.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/google-spreadsheet.png   
          :width: 100
          :alt: 谷歌云文件工具
     - :ref:`谷歌云文件工具`
     - 你可以在你的课程中嵌入一个谷歌云文件,比如文档, 电子表格或图像以便你的学生能在你的课件中看到这个文件.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/GoogleHangout_WithPeople.png   
          :width: 100
          :alt: 谷歌环聊
     - :ref:`谷歌即时环聊`
     - 你可以添加这个工具为了学习你课程的学生参加即时环聊.使用即时环聊学生通过视频和声音可以相互交流,分享屏幕、一起观看和视频协作完成文档。
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/IFrame_1.png
          :width: 100
          :alt: IFrame工具示例示例
     - :ref:`IFrame`
     - IFrame允许你从任何网站和工具不分级别的整合练习和工具到你的课程的一个HTML组件。
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/LTIExample.png
          :width: 100
          :alt: LTI组件示例
     - :ref:`LTI组件`
     - LTI组件允许你添加一个外置的应用程序或者非PDF文本到Studio中.
     - 完全支持
   * - .. image:: ../../../shared/building_and_running_chapters/Images/PA_QandRField.png
          :width: 100
          :alt: 开放回答评估示例
     - :ref:`开放回答评估2`
     - 在开放回答评估中,学生在回答上传不同长度的回答和图像文件会收到不同的回馈.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/PollExample.png
          :width: 100
          :alt: 调查示例
     - :ref:`调查`
     - 你可以在你的课程中发起调查以便你的学生能够分享不同的观点.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/ProblemWithAdaptiveHintExample.png
          :width: 100
          :alt: 自动适配的提示问题示例
     - :ref:`自动适配的提示问题`
     - 一个带有自动适配的提示评估一个学生的回答，然后给学生回馈或基于回答的提示以便这个学生下次一回答更有可能正确回答.这些问题可以是文本输入或多选问题A .
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/ProblemWrittenInLaTeX.png
          :width: 100
          :alt: 用LaTeX写的问题示例
     - :ref:`用LaTeX写的的问题`
     - 如果你有一个已经写入了LaTeX的问题,你可以用这个问题很容易键入转换成XML.
     - 不支持

.. Removed student notes row for now-- cannot conditionalize in tables. Currently student notes page is included in open edx, not in edx.

   * - .. image:: ../../../shared/building_and_running_chapters/Images/TextInputExample.png
          :width: 100
          :alt: 文本输入问题示例
     - :ref:`文本输入问题`
     - 在文本输入问题中, 学生输入文本到回答区域.这个回答可以包括数字，字母和特殊字符比如标点符号.
     - 完全支持  
   
   * - .. image:: ../../../shared/building_and_running_chapters/Images/WordCloudExample.png
          :width: 100
          :alt: word cloud示例
     - :ref:`Word Cloud`
     - Word clouds整理学生输入的文本 - 比如,在回答一个问题 - 变成学生能看见的色彩鲜艳的图形.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/CustomPythonExample.png  
          :width: 100
          :alt: Example write-your-own-grader问题
     - :ref:`Write Your Own Grader`
     - 在自定义的Python-evaluated输入(也叫"write-your-own-grader")
       问题,这个grader使用一个你创建的Python脚本嵌入到这个问题中去评估学生的回复或提供提示embed in
       the problem to evaluates a student's response or provide hints. These
       problems can be any type.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/RecommenderXBlockExample.png
          :width: 100
          :alt: Example RecommenderXBlock
     - :ref:`RecommenderXBlock`
     - RecommenderXBlock可以保留错误修正的列表, 补充说明等等.这个工具允许教师和学生一起维护资源列表.比如,教师和学生可以建立新的资源，为有用的东西投票，或者标记没用的资源和垃圾邮件。
     - 暂时支持  

********************************
图像-基于练习与工具
********************************

.. list-table::
   :widths: 30 25 60 20

   * - .. image:: ../../../shared/building_and_running_chapters/Images/DragAndDropProblem.png
          :width: 100
          :alt: 拖放问题示例
     - :ref:`drag and drop`
     - 在拖放问题中,学生通过拖动文本或对象到一个图像的指定位置回答.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/image-modal.png
          :width: 100
          :alt: 图像全屏工具示例
     - :ref:`全屏图像`
     - 全屏图像工具允许学生放大图像到在整个浏览器中.当这个图像包含大量且详细的文本这是非常有用的，这能让学生看的时候更容易联系上下文.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/ImageMappedInputExample.png
          :width: 100
          :alt: 图像映射输入问题示例
     - :ref:`图像映射输入`
     - 在一个图像映射输入中,学生点击在一个图像中限定的地方点击.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/Zooming_Image.png
          :width: 100
          :alt: 图像放大工具示例
     - :ref:`图像放大`
     - 图像放大工具允许你方法部分图像以便学生能看的更清晰.
     - 完全支持  

************************************
多项选择练习和工具
************************************

.. list-table::
   :widths: 30 25 60 20

   * - .. image:: ../../../shared/building_and_running_chapters/Images/CheckboxExample.png
          :width: 100
          :alt: 复选框问题示例
     - :ref:`复选框`
     - 在复选框问题中,学生选择从可能的是答案的列表中选择一个或多个选项. 学生必须选择所有正确的选项.
     - 完全支持
   * - .. image:: ../../../shared/building_and_running_chapters/Images/DropdownExample.png
          :width: 100
          :alt: 下拉问题示例
     - :ref:`下拉`
     - 下拉问题允许学生从一批答案选项中选择,给出一个下拉列表.和答案总是直接明显的在问题下面的多项选择不同的是,下拉问题不显示选项除非学生点击下拉箭头.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/MultipleChoiceExample.png
          :width: 100
          :alt: 多选问题示例
     - :ref:`多项选择`
     - 在多项问题中，学生从答案列表中选择一个选项.和答案不直接出现在学生视野中的下拉问题不同的是,多选问题的选项总是直观的出现在问题的下面.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/MultipleChoice_NumericalInput.png
          :width: 100
          :alt: 多项选择和数值输入问题示例
     - :ref:`多项选择和数值输入问题`
     - 你可以创建一个多选问题和数值输入问提的问题. 学生不仅仅要选择你提供的答案选项，必要的话，还要提供一个更特殊的答案.
     - 暂时支持  

********************************
STEM练习或工具
********************************

.. list-table::
   :widths: 30 25 60 20

   * - .. image:: ../../../shared/building_and_running_chapters/Images/ChemicalEquationExample.png
          :width: 100
          :alt: 化学方程式问题示例
     - :ref:`化学方程式`
     - 化学方程式问题允许学生输入代表化学房产式的文本到文本框中.grader会用你创建的Python脚本评估学生的回答.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/CircuitSchematicExample_short.png
          :width: 100
          :alt: 电路图生成器问题示例
     - :ref:`电路图生成器`
     - 在电路图生成器问题中,学生可以整理电路原件比如电压、电源、电容、电阻和场效电晶体在一个交互式网络上.他们然后提交一个直流电、交流电或者他们电路的瞬时分析给系统评分.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/GeneExplorer.png
          :width: 100
          :alt: 基因探索问题示例
     - :ref:`基因探索`
     - 基因探索(GeneX)模仿了一个小型真核生物的基因转录, 拼接,加工和翻译.GeneX允许学生做一个基因序列的突变,然后在mRNA和蛋白质上计算并展示突变结果.
     - 暂时支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/MathExpressionInputExample.png
          :width: 100
          :alt:数学表达式输入问题
     - :ref:`数学表达式输入问题`
     - 更复杂的Studio的两种类型的数学问题.在数学表达式输入问题里,学生输入数学表达式去回答一个问题.这些问题可以包含未知的变量和更复杂的符号.你可以指定一个明确的答案或者使用Python脚本.
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/Molecule_Editor.png
          :width: 100
          :alt: 分子编辑器问题示例
     - :ref:`分子编辑器`
     - 分子编辑器允许学生依据共价键的形成和形式电荷规则画分子，即使分子在化学上是不可能的,不稳定的或在生物系统中不存在的.
     -不支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/MoleculeViewer.png
          :width: 100
          :alt: 分子查看器工具示例
     - :ref:`分子查看器`
     - 分子查看器允许你创建一个三维的分子模型让学生观察.
     - No support
   * - .. image:: ../../../shared/building_and_running_chapters/Images/image292.png
          :width: 100
          :alt: 数值输入问题示例
     - :ref:`数值输入`
     - Studio的两种数学问题中教简单的问题.在数字输入问题中,学生输入数字或者或者特殊或简单的数学表达式去回答一个问题.这些问题仅仅允许数字或一些选择 变量. 你可以指定一个错误的范围,你也可以指定一个明确的或用Python脚本的正确答案。
     - 完全支持  
   * - .. image:: ../../../shared/building_and_running_chapters/Images/Periodic_Table.png
          :width: 100
          :alt: 元素周期表问题示例
     - :ref:`元素周期表`
     - 一个交互式的元素周期表显示了关于每种元素的详细信息当学生把鼠标移动到这个元素上时.
     - 不支持
   * - .. image:: ../../../shared/building_and_running_chapters/Images/ProteinBuilder.png
          :width: 100
          :alt: 蛋白质构建器问题示例
     - :ref:`蛋白质构建器
     - 蛋白质构建器会请求学生通过结合氨基酸来形状创建一个特殊的蛋白质形状.
     - 不支持

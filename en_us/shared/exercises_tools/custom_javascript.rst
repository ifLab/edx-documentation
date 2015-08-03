.. _Custom JavaScript:

###########################
自定义JavaScript问题
###########################

自定义JavaScript显示和评分问题(也叫*自定义JavaScript问题* or *JS输入问题*)允许你创建一个自定义问题或工具使用JavaScript然后把这个问题或工具直接添加到Studio.当你创建一个JS输入问题时,
Studio会把这个问题嵌入内联框架(IFrame)以便你的学生可以在LMS里用它进行互动.你可以使用JavaScript和一些基础的Python对你学生的工作进行评分,并且这个分数会整合到edX评分系统中去.

你必须使用HTML，JavaScript和CSS创建JS输入问题.你可以使用任何应用app创作工具,比如Google Web Toolkit (GWT),去创建你的JS输入问题.

.. image:: ../../../shared/building_and_running_chapters/Images/JavaScriptInputExample.png
 :alt: Image of a JavaScript Input problem

.. caution:: 
  你不能在一个包含一个以上问题的组件上使用自定义JavaScript问题.每个自定义JavaScript问题必须在它自己的组件上. 点击 :ref:`Multiple Problems in One Component` 查看更多相关信息.

************************************************************
创建一个自定义JavaScript展示和评分问题
************************************************************

#. 创建你的JavaScript应用，然后上传所有的文件并和那个应用关联到**文件与上传**页面.
#. 当你想要创建这个问题的时候,点击**问题** 在**添加新组件**下方,然后点击**高级**标签.
#. 点击**自定义JavaScript展示和评分**.
#. 在出现的组件里，点击**编辑**.
#. 在这个组件编辑器里，根据你的问题修改示例代码。

   - 所有的问题都有不止一个元素，大多数问题符合同源策略(SOP),意味着所有的元素都有同样的协议，主机和端口.比如, **http**://**store.company.com**:**81**/subdirectory_1/JSInputElement.html和**http**://**store.company.com**:**81**/subdirectory_2/JSInputElement.js有相同的协议(http), 主机(store.company.com), 和端口(81).

     如果你的问题的任何元素使用一个不同的的协议，主机或端口，你需要绕开SOP.比如，**https**://**info.company.com**/JSInputElement2.html使用一个不同的协议，主机和端口。要绕开SOP，在示例代码的第8行把**sop="false"**改成**sop="true"**. 更多信息,请在`Mozilla Developer Network <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Same_origin_policy_for_JavaScript>`_ 或者在 `Wikipedia <http://en.wikipedia.org/wiki/Same_origin_policy>`_看同源策略页面.
#. 如果你想要你的问题有 **保存** 按钮, 点击**设置** 标签, 然后把**最大尝试次数** 设置成一个比0大的整数.
#. 点击**保存**.

================================
重新创建示例问题
================================

要重新创建上面所说的示例问题,你将需要以下的文件.

   - webGLDemo.html
   - webGLDemo.js
   - webGLDemo.css
   - three.min.js

在http://files.edx.org/JSInput.zip可以下载这些文件的.zip压缩文档.

.. note:: 如果你需要绕开SOP,你也需要**jschannel.js**文件,并且你的webGLDemo.html文件会有一些不同.在http://files.edx.org/JSInput_BypassSOP.zip可以下载所有文件.zip文件.

#. 下载并打开JSInput.zip或JSInput_BypassSOP.zip file.
#. 在**文件&上传**页面, 上传zip压缩文档里面的所有文件.
#. 创建一个新的自定义JavaScript展示和评分问题组件.
#. 在**设置**标签, 设置**最大尝试次数**为一个大于0的整数.
#.  在这个组件编辑器里，根据你的问题修改示例代码。用你的代码代替示例代码
#. 点击**保存**

================================
JavaScript输入问题代码
================================

.. code-block:: xml

    <problem display_name="webGLDemo">
    In the image below, click the cone.

    <script type="loncapa/python">
    import json
    def vglcfn(e, ans):
        '''
        par is a dictionary containing two keys, "answer" and "state"
        The value of answer is the JSON string returned by getGrade
        The value of state is the JSON string returned by getState
        '''
        par = json.loads(ans)
        # We can use either the value of the answer key to grade
        answer = json.loads(par["answer"])
        return answer["cylinder"]  and not answer["cube"]
        # Or we can use the value of the state key
        '''
        state = json.loads(par["state"])
        selectedObjects = state["selectedObjects"]
        return selectedObjects["cylinder"] and not selectedObjects["cube"]
        '''
    </script>
    <customresponse cfn="vglcfn">
        <jsinput
            gradefn="WebGLDemo.getGrade"
            get_statefn="WebGLDemo.getState"
            set_statefn="WebGLDemo.setState"
            width="400"
            height="400"
            html_file="/static/webGLDemo.html"
        />
    </customresponse>
    </problem>


.. note::    当你创建这个问题时，请记住以下几点。

 - webGLDemo.js文件定义了三个JavaScript功能(**WebGLDemo.getGrade**, **WebGLDemo.getState**, 和**WebGLDemo.setState**).

 - JavaScript输入问题代码使用**WebGLDemo.getGrade**, **WebGLDemo.getState**, 和**WebGLDemo.setState**去评分,保存,或恢复一个问题.这些函数必须在全球范围内.

 - **WebGLDemo.getState** 和 **WebGLDemo.setState**时可选择的. 你只需要定义这些函数如果你想保存这个问题的状态。

 - **Width** 和 **height** 代表保存在应用程序的IFrame大小。

 - 当这个问题打开时, 圆锥体和立方体都是蓝色的, 或"未选择." 当你点击二者之一, 这个模型会变成黄色, 或"已选择." 要取消选择这个模型,再点一下它.继续点击这个模型会继续选择它.

 - 当用户点击**确定**时如果这个圆锥体被选择(黄色)这个答案会被视作正确答案.

 - 点击**确定**或**保存**保存当前问题的状态.


.. _JS Input Problem XML:

******************************
JavaScript XML输入问题
******************************

JSInput允许问题的作者把独立HTML文件转成可以整合到edX平台的问题. 由于其目的是灵活的,它可以被看作是输入和客户端相当**CustomResponse**.

JSInput练习在一个静态的HTML页面里创建一个IFrame,并把author-specified函数的返回值传递给封闭回答类型(通常是 **CustomResponse**). JSInput也可以保存和回复状态.

========
模板
========

下面是JSInput问题的基本格式:

.. code-block:: xml

 <problem>
        <script type="loncapa/python">
 def all_true(exp, ans): return ans == "hi"
        </script>
        <customresponse cfn="all_true">
            <jsinput gradefn="gradefn" 
                height="500"
                get_statefn="getstate"
                set_statefn="setstate"
                html_file="/static/jsinput.html"/>
        </customresponse>
 </problem>

公认的属性:

==============  ==============  =========  ==========
属性名               类型        是否必要    默认
==============  ==============  =========  ==========
html_file        URL string     Yes        None
gradefn          Function name  Yes        `gradefn`
set_statefn      Function name  No         None
get_statefn      Function name  No         None
height           Integer        No         `500`
width            Integer        No         `400`
==============  ==============  =========  ==========

========================
必要属性
========================


  **html_file**属性指定IFrame将指向的HTML文件.HTML文件必须是位于目录的内容。

  IFrame是使用沙箱属性创建的. 虽然弹出窗口，脚本，允许指针锁定, IFrame不能使用父类属性。

  HTML文件必须包含一个JSInput可以使用的**gradefn**函数. 要确定**gradefn**函数是否可使用,在控制台,确保**gradefn**返回值正确.当JSInput使用**gradefn**函数时, `gradefn`调用`gradefn`.call(`obj`), 在**obj** 是 **gradefn**的部分对象的地方. 比如,如果**gradefn** 是**myprog.myfn**, 则JSInput调用**myprog.myfun.call(myprog)**. (这是确保"`this`"继续指向`gradefn` 期望的.)

 除此之外,或多或少都行. 请注意,目前不支持继承父类的CSS或JavaScript(除了Chrome-只有**seamless** 属性默认设置为真).

* **gradefn**

  The **gradefn**属性指定这个函数的名称，当用户点击**确定**时,这个函数会被调用。并且返回学生的答案.除非**get_statefn**和**set_statefn**属性都被使用了,这个答案作为字符串传递到封闭的回答类型. 在上面的**customresponse**例子里, 这意味着 **cfn** 将可以通过``ans``这个答案.

  当学生尝试提交问题时如果**gradefn**函数抛出异常, 这个提交就无效,这个学生会收到一个通用的提示.这个提示可以通过制作异常的名称``Waitfor Exception``;在这种情况下, 意识信息将是异常信息.

  .. important:: 为了确保学生的最后答案能顺利提交，确保**gradefn**函数不是异步的. 此外, 确保函数返回迅速.学生目前没有迹象表明,她的答案是计算出的。

========================
可选择的属性
========================

* **set_statefn**

  有时一些问题的作者将想要关于学生以前的答案的信息("状态")保存和加载.如果使用**set_statefn**函数, 函数给出它的值将会通过状态作为一个字符串参数, 学生回到一个问题上.这个函数有责任适当的使用这个状态。 The function has the responsibility to then use this state approriately.

  通过的状态:

  * 先前的输出**gradefn** (i.e., 先前的答案) 如果 **get_statefn** 没定义.
  * 先前的输出 **get_statefn** 否则(看下面) .

  iframe负责通过**set_statefn**做适当的验证参数。


* **get_statefn**

  有时状态和答案有很大的不同.比如,一个问题使用javascript程序可能允许学生基于分子的疏水性改变一个分子,但是从疏水性就不能保存这个状态.在这种情况下,*separate*状态可能通过**set_statefn**存和加载.注意如果定义了**get_statefn**,这个答案(i.e., what is passed to the enclosing response type) 将是下面格式的json代码:

  .. code-block:: xml

      {
          answer: `[answer string]`
          state: `[state string]`
      }


  这个封闭的答案类型必须解析这个json.

* **height** 和 **width**

  **height** 和 **width**属性是很简单的: 它们指定IFrame的高度和宽度。它们都被封闭的DOM元素限制,所以有个隐含的最大宽度大约900像素

  将来, JSInput也许会尝试使这些大小匹配HTML文件的尺寸(克服上述的限制),但是现在它默认是高`500`像素，宽`400`像素.



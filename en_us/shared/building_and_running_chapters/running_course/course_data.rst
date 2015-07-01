.. _Course Data:

############################
课程数据
############################

创建课程后，您可以从教师控制面板访问课程相关信息，包括：

* 课程的身份认证信息

* 课程是否已经开始/结束

* 成绩及格/不及格参数

其他课程及学生信息可以从教师面板的其他页面查看，或从edX Insights中查看。
您可以从教师面板中访问Insights：单击某个页面标题中的链接即可。
更多信息请参见 `Using edX Insights`_.

*************************************************
回顾课程数据
*************************************************

如何查看课程数据：

#. 查看课程现况

#. 单击 **导师** → **课程信息**

   **课程基本信息** 区域显示的即为课程的信息列表。

    .. image:: ../../../shared/building_and_running_chapters/Images/Instructor_Dash_Course_Info.png
     :alt: The basic course information section of the Instructor Dashboard 

*************************************************
课程基本信息在Studio中的来源
*************************************************

教师面板中显示的课程数据来源于您在Studio中的设置，或取决于您在Studio中设定的数值。

* **课程运营商**: 在Studio创建课程时设置，属于课程URL的一部分，无法更改。

* **课程号**: 在Studio创建课程时设置，属于课程URL的一部分，无法更改。

* **课程名**: 在Studio创建课程时设置，属于课程URL的一部分，无法更改。
  在Studio中，本字段标签显示为 **课程运营** 。

* **课程显示名**: 在Studio创建课程时设置。在Studio中，本字段显示为 **课程名** 。

  这个名字可以在Studio中更改（如果是直播课程，则不推荐）：
  单击 **设置** → **高级设置** 。**课程显示名** 策略键中的值即为课程在学习管理系统中显示的名称。

  下图显示的是一堂新课程的信息在Studio中的状态，以及在教师面板中 **课程基本信息** 区域内的状态。

.. image:: ../../../shared/building_and_running_chapters/Images/Course_Info_Comparison.png
   :alt: The Course Name in Studio and the Course Display Name in the LMS are boxed; the Course Run in Studio and the Course Name in the LMS are circled
   :width: 800

* **课程是否已经开始**: 取决于 **课程开始日期** 以及当前日期。
  开始日期可以在Studio中更改（如果是直播课程，则不推荐）：
  选择 **设置** → **日程与细节** 。

* **课程是否已经结束**: 取决于 **课程结束日期** 以及当前日期。
  结束日期可以在Studio中更改（如果是直播课程，则不推荐）：
  选择 **设置** → **日程与细节** 。

* **成绩合格参数**: 在Studio中制定评分标准时设置。
  成绩达到标准的学生即通过课程。评分标准可在Studio中更改（如果是直播课程，则不推荐）
  选择 **设置** → **评分标准** 。



.. _Using edX Insights: http://edx-insights.readthedocs.org/en/latest/

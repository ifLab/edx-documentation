.. _Controlling Content Visibility:

###################################
设置内容可见性
###################################

作为教员，您必须认真考虑何时将哪些课程内容对学生开放。

课程内容的可见性取决于以下几点：

* `Release Dates`_
* `Unit Publishing Status`_
* `Content Hidden from Students`_
* `Content Groups`_
  
这些属性将共同控制内容对学生是否可见。

.. _Release Dates:

***********************
发布日期
***********************

您需要为章节和子章节设定发布日期。
默认情况下，子章节与所在章节的发布日期相同，当然，您也可以改变此日期。

指定发布日期后，您可以确认内容是否按计划对学生开放，且未来不需要手动调整此设置。

在发布日期之前，公共单元对学生不可见。
章节和子章节的发布日期不同时，公共单元将在其中较晚的日期之后可见。

发布日期之前，内容对教员可见。
:ref:`previewing the course <Preview Course Content>` 或 :ref:`viewing the live
course as staff<View Your Live Course>`.

请参阅：

* :ref:`Set a Section Release Date`
* :ref:`Set a Subsection Release Date`

***********************
单元发布状态
***********************

发布单元使其对学生可见。如果章节和子章节已经发布，学生将看到最新发布的版本。

学生不会看到未发布的单元，他们也看不到单元中未发布的修改内容或组建。
因此，您可以在不影响学生体验的情况下对已发布的章节进行修改。

更多内容请参阅 :ref:`Unit Publishing Status`.

您可以一次性发布对某个章节或子章节的全部修改，或者只发布对独立单元的修改。
请参考以下内容：

* :ref:`Publish all Units in a Section`
* :ref:`Publish all Units in a Subsection`
* :ref:`Publish a Unit`


.. _Content Hidden from Students:

*****************************
对学生隐藏内容
*****************************

您可以对学生隐藏内容。无论发布状态如何，这些内容将永远对学生不可见。

在某些情况下，您也许希望对学生隐藏单元。例如，某些单元中包含了此章节中其他单元问题的答案。
在问题截至日期之前，您可以设置包含答案的单元不可见。

如果您想将某些单元用于向课程教员提供指导或说明，您也可以对学生隐藏此单元。
只有课程教员能看到这些单元。

您可以隐藏不同等级的内容：

* :ref:`Sections<Hide a Section from Students>`
* :ref:`Subsections<Hide a Subsection from Students>`
* :ref:`Units<Hide a Unit from Students>`

.. note::
 当您
 When you make a previously hidden section or subsection visible to learners,
 some content in the section or subsection may remain hidden. If you have
 explicitly set a subsection or unit to be hidden from learners, this
 subsection or unit remains hidden even when you change the visibility of the
 parent section or subsection. Unpublished units remain unpublished, and
 changes to published units remain unpublished.

.. _Hiding Graded Content:

=====================
Hiding Graded Content
=====================

If you hide a section, subsection, or unit that contains graded problems,
grading is not affected. The hidden problems are still counted when the edX
platform calculates grades. If a problem was at time visible and learners
submitted answers for it, they still receive the credit they earned if you
later hide the problem.

.. _Content Groups:

**************
Content Groups
**************

If you have cohorts enabled in your course, you can use content groups to
designate  particular components in your course as visible only to specific
groups of learners.

For details, see :ref:`About Content Groups` and :ref:`Cohorted Courseware
Overview`.

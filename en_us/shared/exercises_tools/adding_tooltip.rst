.. _Adding Tooltips to a Problem:

====================================
为问题添加提示框
====================================

您可以为问题添加内置提示框，这样当学生将光标移到提示框图标上，可以看到您为帮助他们理解问题所写的文字内容。

例如，在以下问题中，学生将光标移动到提示框图标上，可以看到缩略词“ROI”的定义：

.. image:: ../../../shared/building_and_running_chapters/Images/tooltip.png
 :alt: An example of a tooltip from a learner's point of view.

.. note::
  对于使用屏幕阅读器的学生，当阅读器聚焦在提示框图标上时，提示框将展开并显示提示文字。

要添加提示框，您需要将您想让提示显示的文字内容装在 ``clarification`` 元件里。
例如，以下问题包含两个提示框：

.. code-block:: xml

  <problem>
      <text>
          <p>Given the data in Table 7 <clarification>Table 7: "Example PV
            Installation Costs", Page 171 of Roberts textbook</clarification>,
            compute the ROI <clarification><strong>ROI</strong>: Return on
            Investment</clarification> over 20 years.
          </p>
       . . .

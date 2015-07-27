.. _Conditional Module:

####################
条件模板
####################

********************
格式描述
********************

条件模板的主要标签是 ``conditional``.

.. code-block:: xmltags can contain a correct answer.

    <conditional> ... </conditional>

``conditional`` 可以包含任何模块标签(``html``,
``video``, ``poll``, etc.) 或者 ``show`` 标签.

================
条件式标签
================

是条件模块的一个主要实例.下面的是这种标签的属性.

.. code-block:: xml

    输入源 - 必要的模块位置, 用';'隔开
    [message | ""] - 在提示一个或多个不通过的情况下.你可以使用变量 {link},生成所需的模块链接.

    [submitted] - map to `is_submitted` module method.
    (按下RESET按钮使这个函数返回False.)

    [correct] - 地图到`is_correct`模块方法
    [attempted] - 地图到`is_attempted` 模块方法
    [poll_answer] - 地图到`poll_answer` 模块属性
    [voted] - 地图到 `voted`模块属性
========
显示标签
========

一些到设置模块的符号链接.下面的是这种标签的属性.


.. code-block:: xml

    输入源 - 模板的位置,用';'隔开

*********
示例
*********

========================================
取决于投票的条件句的示例
========================================

.. code-block:: xml

    <conditional sources="i4x://MITx/0.000x/poll_question/first_real_poll_seq_with_reset" poll_answer="man"
    message="{link} must be answered for this to become visible.">
        <html>
            <h2>You see this because your vote value for "First question" was "man"</h2>
        </html>
    </conditional>

========================================================
取决于投票的条件句的示例(使用 <显示> 标签)
========================================================

.. code-block:: xml

    <conditional sources="i4x://MITx/0.000x/poll_question/first_real_poll_seq_with_reset" poll_answer="man"
    message="{link} must be answered for this to become visible.">
        <html>
            <show sources="i4x://MITx/0.000x/problem/test_1; i4x://MITx/0.000x/Video/Avi_resources; i4x://MITx/0.000x/problem/test_1"/>
        </html>
    </conditional>

================================================
取决于问题的条件句的示例
================================================

.. code-block:: xml

    <conditional sources="i4x://MITx/0.000x/problem/Conditional:lec27_Q1" attempted="True">
        <html display_name="HTML for attempted problem">You see this, cause "lec27_Q1" is attempted.</html>
    </conditional>
    <conditional sources="i4x://MITx/0.000x/problem/Conditional:lec27_Q1" attempted="False">
        <html display_name="HTML for not attempted problem">You see this because "lec27_Q1" is not attempted.</html>
    </conditional>

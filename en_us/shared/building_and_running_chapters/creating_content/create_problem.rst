.. _Working with Problem Components:

################################
创建问题组件
################################

******************************
问题组件概况
******************************

问题组件允许您在您课程内容中添加互动式及自动评分的练习。
您可以在Studio下创建不同类型的问题。

通过默认设置，所有问题都会得分，但是不会计算学生的总分。
若您想让这些问题计算学生的总分，修改保存问题的小节的作业类型。

本章讲述的是问题组件的基础知识，即：您与学生所见的视图，每个问题组件的选项。欲知单个问题类型，请见 :ref:`Create Exercises`.

欲知更多信息，请浏览以下主题：

* :ref:`Problem Student View`
* :ref:`Problem Studio View`
* :ref:`Problem Settings`
* :ref:`Modifying a Released Problem`
* :ref:`Additional Work with Problems`
* :ref:`Multiple Problems in One Component`
* :ref:`Problem Randomization`

.. _Problem Student View:

************************************
学生视图下的问题
************************************

凡是出现在edX平台的所有问题均包含以下功能。

.. image:: ../../../shared/building_and_running_chapters/Images/AnatomyOfExercise1.png
 :alt: Image of a problem from a student's point of view, with callouts for 
       elements of the problem

#. **问题文本** 问题文本允许使用任何标准HTML格式。

#. **学生答案填写区域** 学生在此区域输入答案。回答区域的样式随着问题类型而变化。

#. **提交答案** 对于一些问题类型，Studio使用MathJax提交完美的数学公式。

#. **检查按钮** T学生点击检查，查询上交的答案是否争取。若答案正确的话，则出现绿色的打勾符号。

#. **保存按钮** 学生点击保存，保存的是正确的答案，而非提交。因此，学生可回头修改问题的答案。

#. **显示答案按钮** 此按钮是可选择的。学生点击显示答案时，学生能看到正确答案（见上方第2点）和解题说明(见下方第10点）。教师可设置是否开放此功能。

#. **提交答案次数** 教师可设定提交次数限定或不设定提交次数。
   默认情况下，整个课程中所有问题的 **最多尝试次数** 是空值，这表示提交答案次数是无限的。
   如果课程的 **最多尝试次数** 设定为一个特定的值，课程中的每个问题的尝试次数均为这个值，不能设为无限。

   .. image:: ../../../shared/building_and_running_chapters/Images//AnatomyOfExercise2.png
    :alt: Image of a problem from a student's point of view, with callouts for 
          attempts and showing the answer

#. **反馈** 学生点击检查按钮后，所有问题都会显示绿色复选标记或红X。

   .. image:: ../../../shared/building_and_running_chapters/Images//AnatomyofaProblem_Feedback.png
    :alt: Image of feedback checkmark and x from a student's point of view

#. **正确答案** 大多数问题都需要教师指定一个唯一的正确答案。

#. **解析** 教师可以添加一些解析。当学生点击 **显示答案** 按钮时，会显示相关解析。

#. **重置按钮** 此按钮可以清除学生输入的内容，使问题保持原样。
   如果学生已经提交了答案，点击 **重置按钮** 清除已经提交的内容。
   如果问题包含随机变量且随机化设置为 **重置** ，问题中的值将改变。
   如果超过了最多尝试次数，重置按钮将不可见。
   not yet been submitted, and try again to answer the question. If the student


#. **隐藏答案按钮**

   .. image:: ../../../shared/building_and_running_chapters/Images//AnatomyOfExercise3.png
    :alt: A graded assignment shown in the left pane of the LMS for a course

#. **分级** 教师可以决定一组问题是否进行分级。如果一组问题要进行分级的话，课程作业栏就会出现一个钟表图标。

   .. image:: ../../../shared/building_and_running_chapters/Images//clock_icon.png

#. **到期日** 问题是有期限的。过期的问题就不会有检查按钮了，也不能在进行回答或提供回馈了。

.. note:: 问题可以打开或者关闭。关闭的问题没有检查按钮。
          学生仍然可以看见问题，答案和解析，但是不能查看他们自己做的答案，不能提交答案，也不能更改早期的分数。


还有一些题没有立即可见的属性，您可以在Studio中设置这些属性。

*  **随机化** 对于有些问题，教师可以决定是否采用随机生成的方式，这样每个学生的问题都会不同。


*  **问题权重** 在一组特定的问题中，不同问题权重也不同。

*  **标签** 为提高有困难的同学的可访问性，每一个问题都需要有一个描述性标签。
   这个标签通常包含部分或全部的问题文本。大部分的模板会留出标签的位置。您可以在每个题型或者工具类型的文件中找到示例标签。
   

.. _Problem Studio View:

************************************
Studio中的问题视图
************************************

所有的问题都以XML写成。但是，Studio有两个编辑问题的界面：简易编辑器和进阶编辑器。

*  简易编辑器可以让您进行可视化编辑，不必使用XML。

*  进阶编辑器将问题转换为edX的XML标准,您可以直接编辑XML。

通过点击简易编辑器界面右上角的进阶编辑器按钮，您可以随时从简易编辑器切换到进阶编辑器。
但是您不能从进阶编辑器切换到简易编辑器。

.. _Simple Editor:

=================
简易编辑器
=================

当您选择下列问题类型时，简易编辑器将开启并显示一个问题示例。

*  :ref:`Checkbox`: 在复选框问题中，学生在列表答案中，选出一项或多项。

*  :ref:`Dropdown`: 在下拉问题中，学生从下拉列表中选择一个答案。

*  :ref:`Multiple Choice`: 多项选择题要求学生直接从问题下的多个选项中选出一个答案


*  :ref:`Numerical Input`: 数值输入题要求答案只能为整数，分数，普通常量和运算符。

*  :ref:`Text Input`: 在文本输入题中，学生要输入简短文本来回答问题。

下图显示的是简易编辑器中的多项选择题。

.. image:: ../../../shared/building_and_running_chapters/Images//MultipleChoice_SimpleEditor.png
 :alt: The simple editor with numbered callouts for options and an example
     multiple choice problem to demonstrate the formatting.

简单编辑器含有一个工具栏，可将您的问题文本格式化。当您选中文本，点击格式化按钮之后，简单编辑器就可自动将您的文本格式化。

工具栏按钮如下：

1. 创建1级标题
2. 创建多个选项。
3. 创建复选框选项。
4. 创建文本输入选项。
5. 创建数值输入选项。
6. 创建下拉选项。
7. 创建解析，当学生点击显示答案时，就会显示相关解析。
8. 在进阶编辑器中打开问题。
9. 打开格式提示清单。
10. 通过可用标签来识别问题。工具栏选项不可用，但当您使用两对尖角括号指向文本时， 
    前台将此文本显示为问题的可用标签。
    

    此外，edX Insights使用可用标签来确定每个项目中的问题。
    更多信息请参考 `Using edX Insights`_.

.. _Advanced Editor:

===================
进阶编辑器
===================

 **进阶编辑器** 要用XML打开问题。问题模板包括拖拽，下拉和数学表达式，这些都可在进阶编辑器中直接打开。

下图显示的是进阶编辑器中打开的多项选择题。

.. image:: ../../../shared/building_and_running_chapters/Images//MultipleChoice_AdvancedEditor.png
 :alt: Image of a problem in the advanced editor

以下问题模板可在进阶编辑器中打开。

* :ref:`Circuit Schematic Builder` 在电路原理问题中,学生可以在一个交互式网格中创建和修改电路，并提交计算机生成的电路分析来进行分级

* :ref:`Custom JavaScript` 自定义JavaScript显示和分级问题,您可以通过IFrame将之前用HTML制作的题型并入到Studio中。

* :ref:`Drag and Drop` 拖放问题要求学生能够拖动文本或者将文本放到一张图像的指定位置。

* :ref:`Image Mapped Input` 图像映射输入问题要求学生能够点击一张图像上的指定位置。

* :ref:`Math Expression Input` 数学表达式输入问题还要求学生能够输入数学表达式的文本，如e=m*c^2。

* :ref:`Problem with Adaptive Hint` 这些问题会根据学生的答案给予学生一些回馈或提示。

* :ref:`Problem Written in LaTeX` 这类题型能够将您用LaTeX写好的问题转换为edX格式。注意这种题型仍然在试用中，未来可能不再支持这种题型。

* :ref:`Write Your Own Grader` 自定义Python-评估输入（也被称作“自编分级”题型)能够通过您自己创建的嵌入式Python脚本来评估学生的答案。

.. _Problem Settings:

******************
问题设置
******************

除了问题的文本,您使用问题组件创建的问题包括以下设置。这些设置在组件编辑器中的设置选项卡中。

*  `Display Name`_
*  `Maximum Attempts`_
*  `Problem Weight`_
*  `Randomization`_
*  `Show Answer`_
*  `Show Reset Button`_
*  `Timer Between Attempts`_

.. image:: ../../../shared/building_and_running_chapters/Images/ProbComponent_Attributes.png
 :alt: Image of the Settings tab in a Problem component

===============
显示名称
===============

此设置显示您问题的名称。问题名称将以问题标题的形式显示在LMS和页面上方的条状区域。

.. image:: ../../../shared/building_and_running_chapters/Images/ProbComponent_LMS_DisplayName.png
 :alt: Image of the problem in a unit page from a student's point of view

此外，edX Insights 使用显示名称确定每个问题。
唯一且描述准确的显示名将帮助您快速而准确地找到需要分析的问题。
更多信息请参阅  `Using edX Insights`_.

==============================
最多答题次数
==============================

此设置规定学生最多可尝试回答问题次数。系统默认学生的回答次数不受限制。
如果课程范围内的最多答题次数设置为一个特定值，每个问题的默认值也为此特定值，不能将独立问题的值设为无限。

.. note:: 将问题最多回答次数设置为1或者更多，问题才能出现在学生答题统计报告中，您可以在上课时下载该报告。


.. _Problem Weight:

==============================
问题权重
==============================

.. note:: Studio可以保存所有问题的分数，但是只有这些分数属于某个小节，
          并且这个小节被设定成计分后，才会对学生的期末成绩造成影响。

这项设定可以规定问题的最大分值。问题的分值标在在问题题目后面。

.. image:: ../../../shared/building_and_running_chapters/Images/ProblemWeight_DD.png
 :alt: Image of a problem from a student's point of view, with the possible 
       points circled

系统默认，问题组件中的每一个应字段或者“答题框”都值1分。
每一个问题组件都包含多个应字段。
例如，上述问题组件包含一个下拉问题，这个下拉问题包含三个独立问题需要学生来回答，因此它有三个应字段。

下面的问题组件包含一道文本输入题，就只有一个应字段。

.. image:: ../../../shared/building_and_running_chapters/Images/ProblemWeight_TI.png
 :alt: Image of a text input problem from a student's point of view

计算分数
****************

学生回答问题得分由以下公式计算得出：

**分数=问题权重×（正确答案/输入总和）**

*  **分数** 指的是学生回答问题所得的分数。

*  **问题权重** 指的是回答这个问题所能获得的最高分数。

*  **正确答案** 指的是所有回答中正确答案的数量。

*  **输入总和** 指的是所有这个题组本身所拥有的问题数量总和。

**范例**

接下来是一些计算分数的例子。

*范例1*

一个问题的权重属性是空的。这个问题含两个应字段。因为有两个应字段，所以最大分值为2.0分。
 
如果一个应字段中是正确答案，一个应字段是不正确答案，那么这个学生只能得到2分中的1.0分。

*范例2*

一个问题的权重属性为12，有三个字段。

如果一个学生的答案包含2个正确答案和1个错误答案，那么他的分数就是12分中的8分。

*范例3*

一个问题的权重属性为2，有四个应字段。

如果一个学生的答案包含1个正确答案和3个错误答案，那么他的分数就是2分中的0.5分。

.. _Randomization:

===============
随机化
===============

随机化设定可以决定是否要在每次学生看到问题的时候，将其中指定的内容随机化呈现。
例如，每当一个学生提交了一个问题的答案时，后面的问题要随机改变。

.. image:: ../../../shared/building_and_running_chapters/Images/Rerandomize.png
 :alt: The same problem shown twice, with color highlighting on values that 
       can change

如果您想将问题的指定内容进行变更或者随机化呈现，您需要做到以下两点：

* 确保您的问题包含一个Python脚本，能够将您想要的内容进行随机化处理。

* 问题组件内部的随机化处理。

.. note:: 此随机化设置不同于问题随机化处理。随机化设置是在一个问题内部进行随机处理。
 而问题随机化是指将不同问题或者同一问题的不同版本分配给不同的学生。更多信息,请参见
 :ref:`Problem Randomization` 。

置随机化，选择随机化设置选项。此设置含四个选项。

+-------------------+--------------------------------------+
| **总是**          | 学生每次点击检查按钮之后，           |
|                   | 总会看到一个问题的不同版本。         |
|                   |                                      |
+-------------------+--------------------------------------+
| **重置**          | 学生每次点击重置按钮之后，           |
|                   | 总会看到一个问题的不同版本。         |
|                   |                                      |
+-------------------+--------------------------------------+
| **从不**          | 所有学生都会看到问题的同一版本。     |
|                   | 此为系统默认。                       |
+-------------------+--------------------------------------+
| **每个学生**      | 学生个人每次查看，                   |
|                   | 都会看到相同版本的问题，             |
|                   | 但此版本不同于其他学生查看的版本。   |
|                   |                                      |
|                   |                                      |
+-------------------+--------------------------------------+

.. note:: The edX Platform has a 20-seed limit for randomization.

.. _Show Answer:

===============
显示答案
===============

此设置决定何时将答案显示给学生看。此设置含多个选项。

+-------------------+--------------------------------------+
| **总是**          | 学生点击显示答案按钮时，显示答案。   |
+-------------------+--------------------------------------+
| **已回答**        | 在学生回答问题之后显示答案。         |
|                   |                                      |
|                   | 如果问题重置，答案在学生再次回答之   |
|                   | 前不可见。（学生回答问题之后，问题   |
|                   | 为已尝试和已回答状态。               |
|                   | 问题重置之后，问题将是尝试而未解答   |
|                   | 状态。）                             |
+-------------------+--------------------------------------+
| **已尝试**        | 在学生尝试回答问题之后显示答案。     |
|                   |                                      |
|                   | 如果问题重置，答案将持续显示。       |
|                   | （当学生回答问题之后，问题为已尝试   |
|                   | 已回答状态。问题重置之后，问题将是   |
|                   | 尝试而未解答状态。）                 |
+-------------------+--------------------------------------+
| **关闭**          | 学生用完所有的回答问题限制次数或者   |
|                   | 问题过期时，显示答案。               |
+-------------------+--------------------------------------+
| **完成**          | 学生正确回答问题之后，学生用完限制   |
|                   | 回答的次数，或者问题过期，显示答案。 |
+-------------------+--------------------------------------|
| **正确或过期**    | 学生正确回答问题之后，或者问题过期   |
|                   | 显示答案。                           |
+-------------------+--------------------------------------+
| **过期**          | 问题过期时，显示答案。               |
+-------------------+--------------------------------------+
| **永不**          | 永不显示答案。在这种情况下，显示答案 |
|                   | 按钮不会出现在Studio或者LMS的问题    |
|                   | 旁边。                               |
+-------------------+--------------------------------------+

.. _Show Reset Button:

=================
Show Reset Button
=================

This setting defines whether a **Reset** button is visible on the problem.
Students can click **Reset** to clear any input that has not yet been submitted,
and try again to answer the problem. If the student has already submitted an
answer, clicking **Reset** clears the submission and, if the problem contains
randomized variables and randomization is set to **On Reset**, changes the
values the student sees in the problem. If the number of Maximum  Attempts that
was set for this problem has been reached, the **Reset** button is not visible.

This problem-level setting overrides the course-level **Show Reset Button for
Problems** setting.

.. _Timer Between Attempts:

=======================
Timer Between Attempts
=======================

This setting specifies the number of seconds a student must wait between
submissions for a problem that allows multiple attempts. If the value is 0, the
student can attempt the problem again immediately after an incorrect attempt.

Adding required wait time between attempts can help to prevent learners from
simply guessing when multiple attempts are allowed.

If a learner attempts a problem again before the required time has elapsed, she
sees a message below the problem indicating the remaining wait time.

.. image:: ../../../shared/building_and_running_chapters/Images/problem_attempt_timer.png
 :alt: Problem with message that learner must wait before attempting again


.. _Modifying a Released Problem:

*********************************
修改已发布的问题
*********************************

.. warning:: 当您已经发布问题之后，要做修改请务必格外小心！

当学生回答一个问题并提交后，Studio就会保存学生的答案，保存学生得到的分数以及这个问题的最高分。
当学生重新提交答案时，Studio会对这些内容进行更新。
然而，如果教师对问题或者其属性进行变更，Studio无法将学生之前回答的情况进行自动更新。

例如，当您已经发布一个问题，并将答案设置为3。
一些学生提交答案之后，您才发现答案不是3，而是2。
您更改答案后，对于提交了正确答案2的学生，Studio无法更改他们的分数，因此他们的得分是错的。

再举一个例子，您可能将一个问题的2个应字段改为3个应字段。
那么之前提交答案的学生得出的分数可能是0,1或者2分。
同一问题，修改之后提交答案的同学的分数则可能为0,1,2或者3分。

但是，如果您修改了问题的权重属性，刷新进程页面后，现有的分数也会更新。.

===============
工作区
===============

如果您不得不修改一个已经发布的问题，而且会影响分数，有两种方法来解决。
注意，这两种方法都需要您的学生重新回答问题并提交答案。

*  在问题组件中，增加回答问题尝试次数，然后让学生重新答题。

*  删除Studio中的整个问题组件，根据内容和设定，重新创建一个问题组件。
   然后让所有学生回答新的问题。


For information about how to review and adjust student grades in the LMS, see
:ref:`Grades`.

.. _Additional Work with Problems:

************************************
创建问题的其他情况
************************************

当您创建问题时，可能会有多个选项。
您可以在一个问题组件内设置多个问题，或者您可以将一个问题设置成不同学生做不同版本。

.. _Multiple Problems in One Component:

====================================
一个组件内的多个问题
====================================

您可能会创建一个问题，问题答案不只一种。
例如，您想创建一个数值输入的问题，然后创建这个数值输入问题的多个选项。
或者，您想让学生一次查看多个问题的答案。
设置这样的问题，您可以在一个组件内设置多个问题。这些问题可以是不同题型的。

.. note:: 
  You cannot use a :ref:`Custom JavaScript` in a component that contains more
  than one problem. Each custom JavaScript problem must be in its own
  component.

为了在一个组件内建立多个问题，可以新建一个空的进阶问题组件，然后在组件编辑器中为每个问题添加XML。
您只需将XML添加到问题和答案中即可。您不必为其它内容添加代码，比如检查按钮。

检查按钮，显示答案按钮，及重置按钮还有您为问题组件选择的设置，适用于组件内的所有问题中。
因此，如果您将尝试答题次数设置为3，那么学生则有三次机会来回答组件内的整套题，而不是组件内每道题都可以回答3次。
如果学生点击检查，那么LMS就会马上计算本组件内所有问题的得分。
如果学生点击显示答案，那么组件内所有问题的答案都会显示出来。

.. _Problem Randomization:

===========================
问题随机化
===========================

您可能想给不同学生出不同的题，或者同一问题使用不同版本。
您可以用Studio为每个问题或同一问题的每个版本创建一个问题组件，然后对课程进行编辑，以使得学生查看问题时可以随机变化。

请注意在Studio中，问题随机化与随机化设置是不同的。
随机化设置是指一个问题内部的随机变化。
问题随机化是让不同学生能查看不同问题或者同一问题的不同版本。

.. note:: 设置不同版本问题随机变化需要您将您的课程进行输出，在文本编辑器中编辑您课程中的XML文件，然后再将您的课程导入到Studio中。我们建议您操作之前，将您的课程进行备份。如果您对XML编辑不是很熟悉，我们建议您用文本编辑器编辑您的课程。

术语
************

段，节，单元和组件在课程预览视图中与课程导出后文件列表中的名称不同，打开XML文件进行编辑的时候，这些名称也不同。

.. list-table::
   :widths: 15 15
   :header-rows: 0

   * - 课程预览视图
     - 文件列表
   * - 段
     - 章
   * - 节
     - 横向
   * - 单元
     - 纵向
   * - 组件
     - 讨论, HTML, 问题, 或视频

例如，如果您想在您的课程里面找一个特定部分，您打开课程的文件列表，在章节文件夹中查找。要找某一章节，您就查找纵向文件夹。

.. _Create Randomized Problems:

设置随机化问题
****************************

#. 在需要设置随机化问题的单元中，为每一个问题或者每一个问题版本创建一个单独的问题组件。
   例如，您想要做4个问题版本，您就要创建4个单独的问题组件。
   记录一个出现在单元位置的单元识别符字段的32位的单元ID。
   

#. 导出您的课程。相关信息，请查看
   :ref:`Exporting and Importing a Course`。
   保存包含您您课程的记忆位置的.tar.gz文件，这样您就能很容易的找到它。

#. 在文件和文件夹列表中，打开纵向文件夹。

   .. note:: 如果您这一单元还未发布，打开草稿文件夹，然后打开草稿中的纵向文件夹。


#. 在纵向文件夹中，找到与您在第一步中标记的单元ID名称相同的.xml文件，
   在文本编辑器中打开该文件，比如Sublime 2。
   举个例子，如果这个单元ID是e461de7fe2b84ebeabe1a97683360d31，那么您就
   打开e461de7fe2b84ebeabe1a97683360d31.xml这个文件。


   这个文件包含了在这个单元所有的组件，以及这些组件在URL中的名称。
   例如，以下文件包含4个问题组件。


   .. code-block:: xml
     
       <vertical display_name="Test Unit">
          <problem url_name="d9d0ceb3ffc74eacb29501183e26ad6e"/>
          <problem url_name="ea66d875f4bf4a9898d8e6d2cc9f3d6f"/>
          <problem url_name="2616cd6324704f85bc315ec46521485d"/>
          <problem url_name="88987707294d4ff0ba3b86921438d0c0"/>
       </vertical>

#. 为您要进行随机化处理的问题组件添加<随机化> </随机化>标签。

   .. code-block:: xml
      
       <vertical display_name="Test Unit">
         <randomize>
            <problem url_name="d9d0ceb3ffc74eacb29501183e26ad6e"/>
            <problem url_name="ea66d875f4bf4a9898d8e6d2cc9f3d6f"/>
            <problem url_name="2616cd6324704f85bc315ec46521485d"/>
            <problem url_name="88987707294d4ff0ba3b86921438d0c0"/>
         </randomize>
       </vertical>

#. 添加<随机化> </随机化>标签标签之后，保存并关闭.xml文件。

#. 重新将您的课程压缩为a .tar.gz文件。

   了解关于如何在Mac系统中操作的相关信息，请查看 <http://osxdaily.com/2012/04/05/create-tar-gzip/>`_.

   了解关于如何在windows系统操作的相关信息，请查看 <http://stackoverflow.com/questions/12774707/how-to-make-a-tar-gz-on-windows>`_.

#. 在Studio中，再次导入您的课程。

.. note::

  * 一旦您完成了随机化处理，您就只能在Studio中看到一个问题或者一个问题版本。
    您可以在Studio中，直接编辑单个问题，但是若要编辑其他问题，则须将课程进行导出，
    然后在文本编辑器中编辑您的课程。无论教师还是课程团队都要这样操作。
    
  
  * 学生答案生成的.csv文件包含了试题库中学生答的所有问题的答案。

.. include:: ../../../shared/exercises_tools/adding_tooltip.rst

.. _Using edX Insights: http://edx.readthedocs.org/projects/edx-insights/en/latest/

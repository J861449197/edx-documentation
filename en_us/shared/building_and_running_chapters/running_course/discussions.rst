.. _Discussions:


##################################
管理课程讨论项目
##################################

讨论项目，即论坛，旨在构建学生与工作人员，以及学生与学生之间的有效沟通和交流。
创建课程时，您可设立各种讨论课题引导课程参与人员之间的互动，
同时通过运营、管理讨论项目活动鼓励学生参与课程、建立课程社区。

讨论项目（下或称“论坛”）同时也是课程反馈及未来创意的重要来源。

关于运营、协调讨论项目的内容，请参见以下章节：

* :ref:`Overview_discussions`

* :ref:`Organizing_discussions`

* :ref:`Assigning_discussion_roles`

* :ref:`Visibility of Discussion Topics`

* :ref:`Running_discussions`

* :ref:`Moderating_discussions`

* :ref:`Close_discussions`
  
想了解更多关于分队功能对论坛协调事宜的影响，请参考 :ref:`Moderating Discussions for
Cohorts`.

.. note:: The :ref:`Discussions for Students and Staff` section describes
   features that are available to all discussion participants, and might be
   useful to students who are new to online discussion forums. You can share
   the section with your students by, for example, adding a "Never Used a
   Discussion Forum Before?" post that includes the information you think will
   be most useful to them.


.. _Overview_discussions:

********************************
概述
********************************

学生与员工可以通过论坛分享观点、交流看法、交换意见、解决问题。论坛中的互动分为三种。

*  *帖子* 帖子通常用于展开新话题。帖子一般以问题的形式出现，
  要么展开对话，要么引出一个值得关注的问题。您在发帖时，通常将其归类为“提问”或“讨论”。

*  *回复* 回复指的是关于某个帖子问题的直接回答，或某个对话的延续。

*  *评论* 评论指的是针对某条回复的补充说明或边注。
  评论一般不针对整个帖子，只针对某条回复。
 
由帖子、回复、评论组成的对话有时统称为“话题”。

所有员工及参与课程的学生均可发帖、回帖或发表评论，
同时也可以查看其他课程参与者发布的帖子、回复及评语。

课程社区的所有成员，包括员工和学生，均可以赋予论坛协调员或管理员等讨论项目管理职能。
讨论话题可以保存，是课程历史的组成部分。

.. note:: “参与课堂讨论”一章描述了论坛的部分功能，这些功能对所有参加论坛的人都开放，
   对论坛新人而言帮助也很大。对论坛新人而言帮助也很大。
   您可以和学生一起分享其中的内容。
   方式有很多，比如，您可以发一条名为“第一次使用论坛？”的帖子，
   在帖子中提供您认为对学生最有用的信息。

   Discussion administration roles must be explicitly granted to members of
   the course team for them to moderate or administer course discussions. The
   course author, team members with Admin access (Studio), and Instructors
   (Instructor Dashboard) can grant discussion administration roles. For
   information about adding discussion privileges, see
   :ref:`Assigning_discussion_roles`.


.. _Organizing_discussions:

*************************************************
建立课堂讨论课题
*************************************************

edX课程的论坛既可以添加您之前专门为某个课程单元设计好的讨论模块，
也可以开展全课堂范围的讨论课题，比如“课程反馈帖”，“答疑帖”，“技术支持帖”等等。
您可通过Studio添加各种不同类型的讨论课题。


For more information about creating discussion topics, see :ref:`Create
CourseWide Discussion Topics` and :ref:`Create ContentSpecific Discussion
Topics`. For information about configuring discussion topics in courses that
use cohorts, see :ref:`Set up Discussions in Cohorted Courses`.


.. _Create CourseWide Discussion Topics:

=====================================
创建全课堂讨论课题
=====================================

所有课程均包括一个名为“讨论”的页面。创建课程时，
系统会在该页面中默认生成一个名为“General”的讨论课题。

课堂讨论课题，在课堂上引导学生分享、查找信息。
这类课题可以包含“反馈”、“答疑”、“技术支持”等字样。
这类课题的可访问时间与课程的可访问时间一致。

.. note:: Make sure each discussion topic in your course has a unique name,
   whether it is a course-wide topic or a content-specific discussion topic
   that you add as a discussion component. If different discussion topics
   share the same name, learners might be confused as to which discussion
   topic they are participating in. For example, do not add a content-specific
   discussion topic named "General", because a course-wide discussion topic
   named "General" already exists in every course.

如何创建全课堂讨论课题：

#. 在Studio中打开课程 

#. 单击“设置”→“高级设置”

#. 将滚动滑块拖至“讨论课题映射”策略键。系统默认值应为：

 .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_Add_initial.png
  :alt: Policy value of {"General": {"id": "i4x-edX-Open-edx_demo_course"}}

4. 复制“General”后的三行信息，粘贴到结尾的闭大括号前：

 .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_Add_paste.png
  :alt: Policy value of {"General": {"id": "i4x-edX-Open-edx_demo_course"} 
        "General": {"id": "i4x-edX-Open-edx_demo_course"}}

5. 将第二个“General”替换为新课题的名称，注意带上双引号

#. 将第二个“id”值更改为另一个唯一的值。比如，可以为课题名附上一组独一无二的参数

.. note:: In discussion topic IDs, you can use only alphanumeric characters
   and these special characters: underscore, hyphen, and period.

7. 在第一个闭大括号后输入一个逗号

 .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_Add_name.png
  :alt: Policy value of {"General": {"id": "i4x-edX-Open-edx_demo_course"}, 
        "Course Q&A": {"id": "i4x-edX-Open-edx_demo_course_faq"}}

8. 单击“保存更改”。Studio会重新给您输入的值排序并设定格式。
   将滚动条拖回“讨论课题映射”字段，确认输入内容是否已保存。
   如果您在输入时漏掉了标点符号，输入内容不会保存，且没有警告提示。


操作成功后，当学生单击课程的“讨论”页面时，您的课程即出现在下拉列表中。

 .. image:: ../../../shared/building_and_running_chapters/Images/NewCategory_Discussion.png
  :alt: Image of a new topic named Course Q&A in the list of discussions

.. note:: 在分队课堂中，全课堂讨论课题对所有人均可见。
   所有小队中的学生均可访问课题中的帖子及回复。
   您也可以手动将这类课题配置为分队讨论课题。
   详见 :ref:`Coursewide
   Discussion Topics and Cohorts`.

.. _Create ContentSpecific Discussion Topics:

============================================
Create Content-Specific Discussion Topics
============================================

To create a content-specific discussion topic, you add a discussion component
to a unit. Typically, you do this while you are designing and creating your
course in Studio. Follow the instructions in :ref:`Working with Discussion
Components`. The result is a discussion topic associated with a unit and its
content. 

.. warning:: Follow the recommended steps to add discussion components. Do not
   create discussion topics by using the **Duplicate** button in Studio, and
   do not reference the same discussion ID in more than one place in your
   course. Duplicated discussion components will result in discussion topics
   containing the same conversations, even if learners post in different
   discussion topics.

For more information about the visibility of content-specific discussion
topics, see :ref:`Visibility of Discussion Topics`.

.. note:: In courses with cohorts enabled, all content-specific discussion
   topics are divided by cohort when you first add them. Student posts to divided
   discussion topics can only be read and responded to by members of the same
   cohort. You can change the configuration of content-specific discussion topics
   to make them unified and available to all students in the course. See
   :ref:`Content Specific Discussion Topics and Cohorts`.

.. _Assigning_discussion_roles:

*************************************************
安排讨论项目管理职能
*************************************************

您需要指定一个团队帮助您运营讨论项目。

.. note:: 您在Studio中建立的课程团队（或您在教师控制面板中指定的课程工作人员及导师）
   并不默认为论坛管理人员。


   论坛管理人员应由从课程团队中另外指定，其职责是协调、管理课堂讨论项目。
   论坛管理人员可由课程作者、导师（教师控制面板中的）
   或其他有管理权限的团队成员（Studio中的）担任。


论坛管理人员的分类及职能简述如下：

* *论坛协调员* 论坛协调员可以编辑、删除所有消息（包括帖子、回复、评论）；
  可以审核带有“误用信息”标签的帖子；可以封杀、取消封杀帖子；
  可以将帖子置顶；可以批准回复。在帖子列表中，论坛协调员发布的帖子带有“By:staff”字样，
  协调员发表的回复和评论带有加色的“Staff”标识。
  协调员通常从已担任“课程工作人员”的团队成员中选派。

.. removed this clause from 1st sentence per JAAkana and MHoeber: , and, if the
.. course is cohorted, see posts from all cohorts

* *论坛社区助教* 助教的职能和协调员相同。助教发布的帖子带有“By: Community TA”字样，
  发布的评论和回复带有加色的“Community TA”标识。助教通常由学生担任。

.. I put this comment in to make the formatting of this bulleted list consistent when output using the sphinx template

* *论坛管理员* 拥有以上两种职位的所有职能。
  管理员发布的帖子、回复、评论带有相同的“Staff”标识。
  管理员只能由已担任导师的团队成员出任，
  因为管理员除了具有协调员和助教的只能外，还能在必要的时候赋予其他用户论坛管理职能。


安排论坛管理人员时，您需要提供他们的邮箱地址或用户名。

* 如何查看课程团队成员的信息？在教师控制面板中，单击“成员”，
  然后从下拉列表中选择“课程工作人员”/“导师”。

* 如何查看学生信息？在教师控制面板中，单击“数据下载”
  “以CSV格式下载学生资料”


====================================
如何安排职位
====================================

首先，您必须是课程作者，或担任“导师”职位（即，您必须在Studio中有管理权限）。

#. 查看课程现况

#. 单击“导师”→“成员”

#. 在“行政人员列表管理”字段的下拉列表中选择“论坛管理员”、“论坛协调员”或“论坛社区助教”

#. 在用户列表中输入相应的邮箱地址或用户名，单击“添加”


==============
Remove Roles
==============

To remove role privileges from a user, you must be the course author or
an Instructor (that is, you are identified in Studio as a team member with
Admin access or in the LMS as an Instructor).

#. View the live version of the course.

#. Click **Instructor**, then click **Membership**.

#. In the Administration List Management section, use the drop-down list to
   select Discussion Admins, Discussion Moderators, or Discussion Community
   TAs.

#. From the list of users who currently have that role, select the user you
   want to remove, then click **Revoke access**.


.. _Visibility of Discussion Topics:

**********************************
Visibility of Discussion Topics
**********************************

The names that you specify as the category and subcategory names for
discussion components are not visible on the **Discussion** tab until after
the course has started and the unit is released.

However, "seed" posts that you create in content-specific discussion topics
before a course starts or before the unit is released are immediately visible
on the **Discussion** tab, even though the containing category or subcategory
names are not visible. We recommend that you do not create posts in 
content-specific discussion topics before a unit is released. For more
information about release dates and the visibility of components, see
:ref:`Controlling Content Visibility`.

In contrast, :ref:`course-wide discussion topics<Create CourseWide Discussion
Topics>` that you create on the **Advanced Settings** page in Studio,
including the default "General" discussion topic, are immediately visible,
regardless of whether the course has started. They are not associated with any
particular section or subsection of the courseware, and are not subject to
release dates.


.. _Running_discussions:

*********************
运营讨论项目
*********************

讨论项目管理团队可通过多种方式运营论坛，比如在帖子中作贡献、给回复点赞、
认可某条回复等等，他们通过这些方法引导学生发布与话题相关的消息。
下面的几个小技巧能帮助您有效管理讨论项目。

==========================================
编辑讨论帖主题时采用同一的命名规则
==========================================

为区分不同种类的消息，并使消息更方便查找，
您可以指定一系列命名规则以区分不同种类的帖子主题以及回复、评论。如下例：

* 通知变更事宜时可在帖子主题开头加上“[OFFICIAL]”字样

* 提供错误修复信息的帖子的主题可以用“ERRATA”开头

* 告知学生，如果需要课程工作人员帮助时可以在帖子主题中加入“[STAFF]”字样

讨论项目管理团队和学生均可使用这类命名规则以便更有效地搜索信息。

创建新帖子时，必须选择帖子的类型，是“提问”还是“讨论”。
讨论项目团队成员在选择发帖类型时应慎重，同时也应鼓励学生慎重发帖。详见
:ref:`Find Question Posts and Discussion Posts`.

.. future: changing the type of a post, maybe resequence or separate  conventions from post types

========================
为讨论课题做铺垫
========================

为帮助学生学会如何在课堂讨论中尽可能多地收获知识，
教会学生如何根据自己的问题和讨论寻找最佳的讨论课题，
您可以在课程开始之前发几篇帖子作为课堂讨论的“开胃菜”。示例如下：

* 在“General”课题中，发布一条“[INTRO]”帖子，引导学生和员工做自我介绍。

* 您每发布一个讨论课题，第一条帖子应描述如何使用这个课题。
  除了提供指导教程之外，这类“初始消息”还可作为今后学生创建帖子的范例。

We strongly recommend that you do not create seed posts in content-specific
discussion topics before the course starts or before the containing unit is
released. The category and subcategory names for content-specific discussion
topics are subject to the release visibility of their containing unit, and are
not visible until the unit is released. For more details, see :ref:`Visibility
of Discussion Topics`.


======================================
缩小话题范围
======================================

为了鼓励学生多发布更长、更线性化的讨论话题，
少发布大同小异、支离破碎的散帖，论坛管理团队可以试试下面提到的几个技巧。
但是请注意，长篇讨论（通常指回复、评论数量超过200条的讨论）阅读起来有一定难度，
有可能影响学生的课堂体验。


* 帖子置顶。帖子置顶功能可以使某条帖子出现在“讨论”页面中，
  帖子列表的第一条，从而使更多学生能够看见、回复该帖。
  您可以置顶自己写的帖子，也可以置顶其他人的帖子。
  选择“更多”图标，然后点“置顶”即可。

    .. image:: ../../../shared/building_and_running_chapters/Images/Pin_Discussion.png
     :alt: Image of the pin icon for discussion posts

* 给回复点赞。点赞意味着您认为该条回复提供了有价值的信息。
  单击右侧的“√”图标即可。

    .. image:: ../../../shared/building_and_running_chapters/Images/Endorse_Discussion.png
     :alt: Image of the Endorse button for discussion posts

* 将某个问题标记为“已回答”。操作方法同“点赞”。

* 关闭帖子。如果您认为某条帖子很多余，可以在该帖的回复中粘贴一条链接，
  指向您希望学生做出贡献的帖子，然后关闭本条帖子。
  帖子关闭后，无法继续互动。选择“更多”图标中的“关闭”选项即可。

* 通过帖子/回复/评论提供指导信息。您可在全课堂讨论课题的帖子中发布本章第一节中提到的内容，
  也可以设计下一章“edX论坛剖析”中的内容，提示学生何时开始话题，如何回复帖子，如何评论回复。

.. _Moderating_discussions:

***********************
协调论坛工作
***********************

讨论团队成员会随时跟踪监控讨论项目，促使论坛高效运转。
他们也可以从论坛中收集信息，比如学生对哪些知识存在疑问，
对哪部分课程比较感兴趣，等等，并将这些信息转告给课程工作人员。

如果希望培养并维持积极的论坛文化，则需花更多管理时间用于审核、回复论坛内容。
一个大型开放式在线课程的论坛维护时间每周应不少于5小时，
维护工作包括阅读讨论话题、回复、编辑讨论帖，以及和其他讨论团队成员及课程工作人员积极交流。

更多信息请参考
:ref:`Assigning_discussion_roles`.

====================================================
View Profile Information for Discussion Participants
====================================================

If you want to find out more about a specific discussion participant, you can
view that learner's edX profile. Learners can have either a limited profile or a
full profile.

To view a learner's profile, follow these steps.

#. On the **Discussion** page, select a username in a post,
   response, or comment.
#. On the **Active Threads** page for that learner, select the
   learner's username.

The following image shows a learner's username in a post, the learner's
username on the **Active Threads** page, and the learner's profile page.

.. image:: ../../../shared/building_and_running_chapters/Images/SFD_Prof_from_Disc.png
  :width: 600
  :alt: Image of a discussion with a learner's username circled, an image of
      that learner's active threads page in the course discussions, and an
      image of the learner's profile

For more information, or to create your own profile, see `View, Create, or
Edit an edX Profile <http://edx- guide-for-
students.readthedocs.org/en/latest/sfd_your_information.html#sfd_pro
file_page>`_.

========================================
为学生提供指导
========================================

关于如何参与论坛活动，您可以选取几个最佳案例作为模范，
然后以课程讲义文件的形式发放给学生，或在课程中单独开一个页面详述。
您可以通过这些指南表达自己对学生的期望，也可以介绍edX论坛的功能。

您也可以选择将 :ref:`Discussions for Students and Staff` 一章中的内容与学生共享。
它描述了讨论参与者可以使用的所有功能，即使是论坛新手也可以从中受益良多。

.. For a template that you can use to develop your own guidelines, see
.. :ref:`Discussion Forum Guidelines`.

========================================
培养积极的论坛文化
========================================

论坛管理者可以通过优化论坛互动行为，使论坛传播积极影响，最大化地利用讨论时间。

* 鼓励学生做出高质量的贡献：应该感谢那些发布积极帖子的学生以及踊跃回答问题的学生。

* Check links, images, and videos in addition to the text of each message. Edit
  offensive or inappropriate posts quickly, and explain why.

* 审阅点赞人数较多的帖子，定期、公开地评选“明星楼主”。

* 紧扣主题：请先读完帖子，再发表回复。

* 保持积极的态度：发现问题和错误时，不应指责抱怨。

* 及时回复：作业、小测验等重要事件的截止日期将近时，应多花时间回答论坛中提出的问题。

* 尽量减少赘余的帖子：在回复帖子之前，应看看有没有其他内容类似的帖子。
  回复最紧扣主题或最活跃的帖子，并复制其URL用来回复其他类似的话题。

* 将论坛中的问题公开发布：将问题和答案分享到FAQ课题中，或在“课程信息”页面中公布。

本节内容的模板详见 :ref:`Guidance for Discussion Moderators`.

.. _Find Question Posts and Discussion Posts:

==========================================
查找提问和讨论
==========================================

学生创建新帖子时需指定帖子的类型，是寻找准确的信息（提问）？
还是开始一场开放性的对话（讨论）？

在“讨论”页面中，提问帖通常带有“问号”标记，讨论帖带有“对话气泡”标记。
当提问帖的问题得到解决，且答案被采纳，问号标记自动变成“√”标记。详见 :ref:`Answer
Questions`.

除了通过这些标记辨别之外，您还可以通过论坛的筛选功能查找之前的提问帖和讨论帖。
在“讨论”页面上方，筛选条件默认为“所有帖子”。您也可以将其更改为：

* **未读** ，指的是所有您没有阅读过的帖子，包括提问帖和讨论帖。

* **未解决** 指的是仍然没有最佳答案的提问帖。

==================
编辑消息
==================

三种论坛管理职能均有权编辑和更改帖子、回复和评论的内容
。一旦发现泄露机密、泄露答案，或含有不良信息、偏离主题信息的内容，
应及时删除其文本、图片和链接。

#. 登录官网，在“当前课程”面板中选择相应课程

#. 打开“讨论”页面，打开需要编辑的帖子。
   您可以从下拉列表中选择，也可以通过筛选功能及搜索功能快速定位帖子

#. 找到需要修改的内容后，单击右侧的“更多”图标，选择“编辑”

#. 直接删除有问题的部分，可以附上一行字：“该内容已被管理员删除”

#. 交代删除原因。例如，“含有违背道德准则的信息”

==================
删除消息 
==================

三种论坛管理职位均有权删除帖子、回复及评论的内容。
含有垃圾信息以及不文明用语的帖子应直接删除。


#. 登录官网，在“当前课程”面板中选择相应课程

#. 打开“讨论”页面，打开需要编辑的帖子。您可以从下拉列表中选择，
   也可以通过筛选功能及搜索功能快速定位帖子

#. 找到需要删除的内容。单击右侧的“更多”图标，选择“删除”

#. 单击“OK”

.. how to communicate with the poster?

.. important:: 若发现帖子内容含有威胁性或强烈攻击性的内容，请联系所在学院的校园保卫处，
  报告事件后再考虑采取进一步行动。

==================================
批复不良信息报告
==================================

学生有权上报他们认为含有不良信息的内容。
三种论坛管理职位均可查证这些内容，必要时可以编辑或删除该内容。

#. 查看课程现况，单击页面顶部的“讨论”面板

#. 页面左侧显示的是帖子列表，使用筛选列表，选择“被标记的帖子”

#. 重新查看帖子列表，此时列表中显示的是内容（包括评论、回复）被举报的帖子。
   被举报的内容会带有“被举报”标识

#. 重新审核帖子，编辑或删除相关内容，或者取消举报标记：
   单击“更多”，选择“取消举报”。

===============
冻结账户
===============

如果发现有学生持续发布不良内容，您可以开除该学生。详见 :ref:`unenroll_student`. 
如果课程招生时间已过，该生将无法重新参与课程。

.. _Close_discussions:

******************************
关闭论坛
******************************

您可以关闭课程论坛，关闭后，学生无法继续发布信息。
论坛可以暂时关闭，譬如在考试的时候，也可以永久关闭，譬如在课程结课的时候。

关闭论坛后，所有课程单元中的讨论课题以及全课堂讨论课题均会受到影响。

* 已经发布的讨论、贡献内容仍然保留。
  
* 论坛关闭后，学生无法发帖、回复、评论，
  但是可以继续为已发布的帖子及收藏的帖子点赞，
  也可以举报不良信息。

* 关闭论坛后，课程工作人员、导师、论坛管理员、论坛协调员、
  论坛社区助教等职位的职能不受影响。这些职位可以继续发布讨论内容。

.. note:: 关闭论坛后，学生无法继续讨论。为使学生理解这种情况， 
  您可在“课程信息”页面通知论坛关闭日期，并将该日期挂到“General”讨论课题下。

=====================================
开始-停止日期格式规范
=====================================

您需要在Studio中设置论坛开始关闭与停止关闭的时间。请按下面的格式输入对应值:

``["YYYY-MM-DDTHH:MM", "YYYY-MM-DDTHH:MM"]``

其中：

* 您输入的日期与时间应为世界标准时间，而非您所在时区时间。

* 数字日期与小时之间用大写字母T分隔。

* 第一个时间是论坛开始关闭的时间。

* 第二个时间为论坛重新开放的时间。

* 如果您希望永久关闭论坛，输入一个远在天边的日期即可。

* 不要忘记双引号。

* 开始与结束时间之间用逗号分隔。

* 不要忘记方括号。

* 您可以输入多个开始-结束时间对，每对时间之间用逗号加一个空格分隔。

例如，如果您希望在七月份的期末考试期间暂时关闭论坛，
然后在2014年8月9日永久关闭论坛，输入如下两组数值：

``["2014-07-22T08:00", "2014-07-25T18:00"], ["2014-08-09T00:00", "2099-08-09T00:00"]``

每对方括号仅表示一组时间对。

============================================
设置论坛关闭时间
============================================

步骤：

#. 在Studio中打开课程

#. 选择“设置”→“高级设置”

#. 将滚动条拖至“论坛关闭日期”策略键

#. 在策略键后的区域内，将光标放在已有的两个方括号之间。
   输入一个或多个开始-结束时间对，注意一定要采用之前提到的格式规范。

   如果您输入上面例子中提到的日期，则出现下图：

   .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_blackout_unformatted.png
     :alt: Policy value of [["2014-07-22T08:00", "2014-07-25T18:00"],
         ["2014-08-09T00:00", "2099-08-09T00:00"]]

5. 单击“保存”

   系统会将您输入的数据重组，加入换行符和缩进符，如图示：

   .. image:: ../../../shared/building_and_running_chapters/Images/Discussion_blackout_formatted.png
     :alt: Same policy value but with a line feed after each bracket and comma,
         and an indent before each date

您需要发邮件提醒学生论坛关闭和开启的时间，详见 :ref:`Example Messages to
Students`.

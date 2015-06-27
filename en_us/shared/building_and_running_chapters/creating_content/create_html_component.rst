.. _Working with HTML Components:


#############################
如何使用HTML组件
#############################

***********************
HTML组件概述
***********************

HTML，即超文本标记语言，是构建网页的基本标记语言。
网页浏览器的功能就是将HTML编码以更可读的格式呈现。

也就是说，当学生看见您在课堂上发布的文本或图片时，实际上看的是浏览器格式化后呈现的HTML编码。
更多关于HTML的信息请参考维基百科。 `Wikipedia <http://en.wikipedia.org/wiki/HTML>`_.

HTML组件是您创建课程内容时的主要元素。
您可使用HTML组件添加并格式化文本、链接、图像等等。
您可以选择直接用HTML编码创建HTML组件，或者使用可视化编辑器，该工具会隐藏HTML编码的细节，这在后面的教程中会提到。

更多信息请参考以下章节：

* :ref:`Options for Editing HTML Components`
* :ref:`The Visual Editor`
* :ref:`The Raw HTML Editor`
* :ref:`HTML Component Templates`
* :ref:`Create an HTML Component`
* :ref:`Add a Link in an HTML Component`
* :ref:`Add an Image to an HTML Component`
* :ref:`Import LaTeX Code`

.. note:: 
 在开始创建HTML组件之前，请先回顾 :ref:`Developing Your Course Index` 和 :ref:`Best Practices for HTML
 Markup` 中的内容。

若想给HTML组件添加快速搜索框，参考 :ref:`Google Instant
Hangout` 。


.. _Options for Editing HTML Components:

********************************************
HTML组件编辑选项
********************************************

您可以用以下两种方法操作HTML：

* :ref:`The Visual Editor`
  
  您可使用可视化编辑器，通过一个类似文字处理的界面创建、编辑或格式化课程内容，而不需要直接使用HTML编码。
  使用该编辑器，您可以更方便地格式化内容，或给内容添加链接和图像。
  同时，该编辑器支持HTML编码，因此可以在格式化的过程中作出细小的改变。
  不过，视觉化编辑器与原始HTML编辑器不同，前者中的HTML无法进行细节控制，同时也不支持自定义格式化或自定义脚本。

* :ref:`The Raw HTML Editor`

  在该编辑器中，您可直接使用HTML编码进行操作，同时可使用自定义格式化以及脚本模式。


为HTML组件设置编辑器
************************************

您可在 **设置** 标签下为HTML组件设定一个编辑器：

.. image:: ../../../shared/building_and_running_chapters/Images/set_html_editor.png
 :alt: The Editor selection drop-down list in the HTML Component Settings tab

选择 **可视化编辑器** 或 **原始编辑器** 。当更改编辑器时，需单击 **保存** ，然后重新打开组件才能开始使用新的编辑器。

.. warning:: 
 如果您原本在使用原始HTML编辑器，然后突然切换到可视化编辑器，那么您将丢失已经创建的自定义HTML内容。
 因此，如果您需要创建自定义HTML内容，建议您先使用可视化编辑器，然后再切换到原始编辑器。

.. _The Visual Editor:

*****************************************
可视化编辑器
*****************************************

可视化编辑器的处理界面有“所见即所得”的功能。您可单击编辑器顶部的格式编辑按钮以格式化文本。

.. image:: ../../../shared/building_and_running_chapters/Images/HTMLEditor.png
 :alt: Image of the HTML component editor

.. note:: 
  The visual editor is not available for :ref:`course handouts <Adding Course Updates and Handouts>`.

The following image shows call-outs for the editing options and is followed by
descriptions.

.. image:: ../../../shared/building_and_running_chapters/Images/HTML_VisualView_Toolbar.png
  :alt: Image of the HTML editor, with call-outs for formatting buttons

#. 为选中的段落选择格式风格，如标题1、标题2，等等；
#. 为选中的文本设置字体，如Arial, Courier New, Times New Roman等；
#. 加粗；
#. 斜体；
#. 下划线；
#. 文字颜色
#. 以编码形式格式化文本；
#. 插入项目符号；
#. 插入项目编号；
#. 添加/删除缩进符；
#. 将选中段落设置为引用格式；
#. 为选中的文本添加链接，详见“在HTML组件中添加链接”的内容；
#. 删除当前链接；
#. 在光标位置插入图像，详见 :ref:`Add an Image to an HTML Component`.
#. 使用HTML源代码，详见后文。


.. _Work with HTML code:


Work with HTML code in the Visual editor
*****************************************

To work with HTML source code for the content you create in the visual editor,
click **HTML**  in the editor toolbar. The HTML source code editor opens:

.. image:: ../../../shared/building_and_running_chapters/Images/HTML_source_code.png
 :alt: Image of the HTML source code editor

Edit the HTML code as needed. 

You should not add custom styles or scripts in the HTML code view in the
visual editor. Use the raw HTML editor instead.

Click **OK** to close the source code editor and apply your changes in the
visual editor. The visual editor then attempts to ensure the underlying HTML
code is valid; for example, if you do not close a paragraph tag, the editor
will close it for you.

.. warning:: 
 Clicking **OK** in the source code editor does not save your changes to the
 HTML component.  You return to the component editor, where your changes are
 applied.  You must then also click **Save** to save your changes and close the
 component. If you click **Cancel**, the changes you made in the HTML source
 code are lost.

.. _The Raw HTML Editor:

*****************************
The Raw HTML Editor
*****************************

When you select the raw editor for the HTML component, you edit your content in
a text editor:

.. image:: ../../../shared/building_and_running_chapters/Images/raw_html_editor.png
 :alt: The raw HTML editor

You must enter valid HTML. The raw HTML editor does not validate your HTML code.
Therefore you should thoroughly test the HTML content in your course.


.. _HTML Component Templates:

*****************************
HTML Component Templates
*****************************

When you create a new HTML component, you select from a list of templates:

.. image:: ../../../shared/building_and_running_chapters/Images/html_templates.png
 :alt: The list of HTML Component templates

The raw HTML template is set to use the raw HTML editor. All other templates
use the visual editor.

For any HTML component, you can change the editor, regardless of the template
used to create the component. See `Set the Editor for an HTML Component`_.



.. _Create an HTML Component:

*****************************
Create an HTML Component
*****************************

To create an HTML component:

1. Under **Add New Component**, click **HTML**.

  .. image:: ../../../shared/building_and_running_chapters/Images/NewComponent_HTML.png
   :alt: Image of adding a new HTML component

2. Select the template. 

   The rest of these instructions assume you selected
   **Text**, which creates an empty component with the visual editor selected.

   An empty component appears at the bottom of the unit.

  .. image:: ../../../shared/building_and_running_chapters/Images/HTMLComponent_Edit.png
   :alt: Image of an empty HTML component

3. In the component, click **Edit**.

   The HTML component opens in the visual editor.

  .. image:: ../../../shared/building_and_running_chapters/Images/HTMLEditor_empty.png
   :alt: Image of the HTML component editor

4. Enter and format your content. You can :ref:`Work with HTML code` if needed.

5. Enter a display name (the name that you want students to see). To do this,
   click **Settings** in the upper-right corner of the component editor, and
   then enter text in the **Display Name** field.

   To return to the text editor, click **Editor** in the upper-right corner.

6. Click **Save** to save the HTML component.

When using the visual editor, you can also:

* :ref:`Add a Link in an HTML Component`
* :ref:`Add an Image to an HTML Component`
* :ref:`Import LaTeX Code`

.. _Add a Link in an HTML Component:

***********************************
Add a Link in an HTML Component
***********************************

When using the visual editor, to add a link to a website, course unit, or file
in an HTML component, you work with the **Insert link** dialog box.

.. image:: ../../../shared/building_and_running_chapters/Images/HTML_Insert-EditLink_DBox.png
 :alt: Image of the Insert link dialog box

You can:

* :ref:`Add a Link to a Website`
* :ref:`Add a Link to a Course Unit`
* :ref:`Add a Link to a File`

.. _Add a Link to a Website:

Add a Link to a Website
***********************************

To add a link to a website:

#. Select the text that you want to make into the link.

#. Click the link icon in the toolbar.

#. In the **Insert link** dialog box, enter the URL of the website that you
   want in the **URL** field.

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_Insert-EditLink_Website.png
    :alt: Image of the Insert link dialog box

#. If you want the link to open in a new window, click the drop-down arrow next
   to the **Target** field, and then select **New Window**. If not, you can
   leave the default value.

#. Click **OK**.

#. Save the HTML component.

#. To test the link, click **View Live Version** or **Preview**. When the unit
   opens in the LMS, click the linked text and verify that the correct URL
   opens.

   Note that if your link is to another HTML component in the course, the unit
   of that destination component must be published for the link to work.


.. _Add a Link to a Course Unit:

Add a Link to a Course Unit
***********************************

You can add a link to a course unit in an HTML component.

#. Obtain the unit identifier of the unit you're linking to. To do this, open
   the unit page in Studio, and copy the unit ID from the **Unit Identifier**
   field under **Unit Location** in the right pane.
   
   .. image:: ../../../shared/building_and_running_chapters/Images/UnitIdentifier.png
    :alt: Image of the unit page with the unit identifier circled

#. Open the HTML component where you want to add the link.

#. Select the text that you want to make into the link.

#. Click the link icon in the toolbar.

#. In the **Insert link** dialog box, enter the following in the **URL** field.

   ``/jump_to_id/<unit identifier>``

   Make sure to replace <unit identifier> (including the brackets) with the
   unit identifier that you copied in step 1, and make sure to include both
   forward slashes (/).

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_Insert-EditLink_CourseUnit.png
    :alt: Image of the Insert link dialog box with a link to a unit identifier

  .. caution::
    Ensure you use ``/jump_to_id/<unit identifier>`` as the URL value. Do not
    use the URL of the unit that you see in the browser address bar.  If you do
    not use ``/jump_to_id/<unit identifier>``, the link will be broken if you
    export then import the course.

6. If you want the link to open in a new window, click the drop-down arrow next
   to the **Target** field, and then select **New Window**. If not, you can
   leave the default value.

#. Click **Insert**.

#. Save the HTML component and test the link.

.. _Add a Link to a File:


Add a Link to a File
***********************************

You can add a link in an HTML component to any file that is uploaded for the
course. For more information about uploading files, see :ref:`Add Files to a
Course`.

.. tip:: 
 When adding links to files, open the HTML component and the **Files &
 Uploads** page in separate browser windows. You can then more quickly copy and
 paste file URLs.

#. On the **Files & Uploads** page, copy the **Studio** URL of the file.

  .. image:: ../../../shared/building_and_running_chapters/Images/HTML_Link_File.png
   :alt: Image of Files and Uploads page with the Studio URL field circled 
  
  .. note:: 
   You must use the **Studio** URL to link to the file, not the **Web** URL.

2. In the HTML component where you want to add the link, select the text that
   you want to make into the link.

#. Click the link icon in the toolbar.

#. In the **Insert link** dialog box, enter the Studio URL for the file in the
   **URL** field.

   ``/static/{FileName}.{type}``

   Make sure to include both forward slashes (/).

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_Insert-EditLink_File.png
    :alt: Image of the Insert link dialog box with a link to a file

#. If you want the link to open in a new window, click the drop-down arrow next
   to the **Target** field, and then select **New Window**. If not, you can
   leave the default value.

#. Click **Insert**.

#. Save the HTML component and test the link.

.. _Add an Image to an HTML Component:

***********************************
Add an Image to an HTML Component
***********************************

When using the visual editor, you can add any image that you have uploaded for
the course to an HTML component. For more information about uploading images,
see :ref:`Add Files to a Course`.

Review :ref:`Best Practices for Describing Images` before you add images to
HTML components.

.. note:: 
 Ensure that you obtain copyright permissions for images you use in
 your course, and that you cite sources appropriately.

To add an image, you'll need the URL of the image that you uploaded to the
course. You'll then create a link to the image in the HTML component.

.. tip:: 
 When adding images, open the HTML component and the **Files &
 Uploads** page in separate browser windows. You can then more quickly copy and
 paste image URLs.

#. On the **Files & Uploads** page, copy the **Studio** URL of the image that
   you want. For an example illustration, see :ref:`Add a Link to a File`.

  .. note:: 
   You must use the **Studio** URL to add the image, not the **Web** URL.

2. In the HTML component where you want to add the link, click the image icon
   in the toolbar.

#. In the **Insert image** dialog box, enter the Studio URL for the file in the
   **URL** field.

   ``/static/{FileName}.{type}``

   Make sure to include both forward slashes (/).

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_Insert-Edit_Image.png
    :alt: Image of the Insert image dialog box with a reference to a file

4. Enter alternative text in the **Image description** field. This text becomes
   the value of the ``alt`` attribute in HTML and is required for your course
   to be fully accessible. See :ref:`Best Practices for Describing Images` for
   more information.

#. As needed, customize the image dimensions. Keep **Constrain proportions**
   checked to ensure the image keeps the same width and height proportions. 

   With **Constrain proportions** selected, you only change one dimension. When
   you tab out of the field, the other dimension changes to a value that
   maintains the same image proportions.

#. To change the spacing and border of the image, click the **Advanced** tab. 

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_Insert-Edit_Image_Advanced.png
    :alt: Image of the Insert image dialog box Advanced tab

#. Enter the **Vertical space**, **Horizontal space**, and **Border** as
   needed. The values you enter are automatically added to the **Style** field.

#. Click **OK** to insert the image in the HTML component.

#. Save the HTML component and test the image.


.. _Import LaTeX Code:

****************************************
Import LaTeX Code into an HTML Component
****************************************

You can import LaTeX code into an HTML component. You might do this, for
example, if you want to create "beautiful math" such as the following.

.. image:: ../../../shared/building_and_running_chapters/Images/HTML_LaTeX_LMS.png
 :alt: Image of math formulas created with LaTeX

.. warning:: 
 The LaTeX processor that Studio uses to convert LaTeX code to XML is a third-
 party tool. We recommend that you use this feature with caution. If you do use
 it, make sure to work with your Program Manager.

This feature is not enabled by default. To enable it, you have to change the
advanced settings in your course.

To create an HTML component that contains LaTeX code:

#. Enable the policy key in your course.

   #. In Studio, click **Settings**, and then click **Advanced Settings**.
   #. In the field for the **Enable LaTeX Compiler** policy key, change
      **false** to **true**.
   #. At the bottom of the page, click **Save Changes**.

#. In the unit where you want to create the component, click **html** under
   **Add New Component**, and then click **E-text Written in LaTeX**. The new
   component is added to the unit.

#. Click **Edit** to open the new component. The component editor opens.

  .. image:: ../../../shared/building_and_running_chapters/Images/latex_component.png
   :alt: Image of the HTML component editor with the LaTeX compiler.

4. In the component editor, click **Launch Latex Source Compiler**. The LaTeX
   editor opens.

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_LaTeXEditor.png
    :alt: Image of the HTML component editor with the LaTeX compiler

#. Write LaTeX code as needed. You can also upload a LaTeX file into the editor
   from your computer by clicking **Upload** in the bottom right corner.

#. When you have written or uploaded the LaTeX code you need, click **Save &
   Compile to edX XML** in the lower-left corner.

   The component editor closes. You can see the way your LaTeX content looks.

   .. image:: ../../../shared/building_and_running_chapters/Images/HTML_LaTeX_CompEditor.png
    :alt: Image of the LaTeX component

#. On the unit page, click **Preview** to verify that your content looks the
   way you want it to in the LMS.

   If you see errors, go back to the unit page. Click **Edit** to open the
   component again, and then click **Launch Latex Source Compiler** in the
   lower-left corner of the component editor to edit the LaTeX code.

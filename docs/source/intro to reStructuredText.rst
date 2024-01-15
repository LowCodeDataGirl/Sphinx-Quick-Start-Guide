Introduction to ReStructured Text

Restructured Text is a plain text markup language. Its simplicity and readability make it an excellent choice for writing software documentation. Sphinx extends reST with several unique features, making it more powerful for documenting software projects.
Why reStructuredText?
- - - - - - - - - - - - 
Simplicity and Readability: reST's syntax is intentionally designed to be simple and human-readable. This simplicity ensures that the source text is easily understandable, making documentation maintenance more straightforward.
Powerful and Flexible: Despite its simplicity, reST is powerful. It supports a wide range of formatting options and is extensible, making it suitable for complex documentation needs.
Versatile Output Formats: Sphinx can convert reST documents into various formats such as HTML, PDF, and ePub, making your documentation accessible in different mediums.
Extensibility for Technical Documentation: Sphinx extends reST with special directives and roles specifically designed for technical documentation, such as the automatic generation of code documentation.
Widely Used in the Python Community: reST is particularly popular in the Python community, making it a standard choice for documenting Python projects. However, its use extends well beyond Python, serving various documentation needs across different programming languages and projects.
Environment Setup for reStructuredText
Install Sphinx: Ensure Sphinx is installed in your Python environment as it processes .rst files.
Choose a Text Editor: While any text editor works, using one with reST support (like VS Code, Sublime Text, or Atom) will make your writing process smoother.

Creating Your First .rst File
Choose a Directory: Typically, .rst files are placed in a docs directory in your project.
Create the File: Start with something simple, like introduction.rst.
Naming Conventions: Name your files meaningfully. For example, installation_guide.rst for installation instructions.

Basic Principles of reStructuredText
reStructuredText is all about simplicity and readability. It uses simple syntax for formatting:
Plain Text: Write your content in plain text.
Whitespace and Indentation: Use line breaks and indentation to structure your document.
Simple Markup: Use uncomplicated markup for formatting (like asterisks for bold and underscores for links).

Basic Syntax of reStructuredText
reStructuredText (reST) is designed to be quick to read and write, making it ideal for documentation. Here are some key elements of its syntax:
1. Headings and Sections
Headings in reST are created using underlines (and optionally overlines) made up of different characters. The choice of character doesn't matter, but consistency within a document is essential. The underline (or overline and underline) length should match the length of the heading text. Here's an example:
=================
Chapter 1: Basics
=================

Section Heading
---------------

Subsection Heading
~~~~~~~~~~~~~~~~~~
Paragraphs
Paragraphs in reStructuredText are just blocks of consecutive lines of text, separated by one or more blank lines. For example:
This is a paragraph. It contains several sentences.

This is another paragraph. It's separate from the first one.
Lists
Lists are a great way to present information. reST supports both ordered (numbered) and unordered (bullet) lists.
Unordered Lists: You can create bullet lists using asterisks, plus signs, or hyphens. They are interchangeable, but it's good practice to stick to one type for consistency.

* Item One
* Item Two
  * Subitem One
  * Subitem Two
Ordered Lists: For ordered lists, use numbers followed by a period.
1. First Item
2. Second Item
 
Literal Blocks
For code or other text where line breaks need preserving, use a literal block. Indent each line of the block with a consistent amount of space:
:: 

    This is a literal block.
    Every line is preserved.
 
 
Directives
Directives are a powerful feature in reStructuredText for adding specialized content. They are indicated by .. followed by the directive type and two colons, like:
.. image:: path/to/image.jpg
   :alt: an example image
Adding Elements in reStructuredText
Enhancing your documentation with different elements not only makes it more informative but also engaging and user-friendly. In reStructuredText (reST), you can easily add various elements like images, links, code blocks, tables, and special text blocks.
Images
Inserting images is straightforward in reST. You can include an image using the .. image:: directive followed by the path to the image. Optional attributes like :alt: for alternative text, :height:, :width:, and :align: can also be used
.. image:: path/to/image.jpg
   :alt: A descriptive text for the image
   :align: center
For internal links, you can reference a section or a document within your Sphinx project:
`Link to a section <#section-label>`_
`Link to a document <document-name.rst>`_
Code Blocks
Including code blocks can be vital for technical documentation. In reST, you can use the .. code-block:: directive, specifying the programming language for syntax highlighting:
.. code-block:: python

   def example_function():
       print("This is a code block")
For unhighlighted code, a simple indented block will suffice:
::

    Unhighlighted code block
Tables
Tables can be created using simple grid-like formats or the more advanced list-table directive:
Simple Grid Table:

+------------+------------+
| Header 1   | Header 2   |
+============+============+
| Cell 1     | Cell 2     |
+------------+------------+
List Table:

.. list-table::
   :header-rows: 1

   * - Header 1
     - Header 2
   * - Row 1, Cell 1
     - Row 1, Cell 2
Admonitions
Admonitions are special blocks used for notes, warnings, tips, etc., that help to highlight important information:
.. note:: This is a note.
.. warning:: Important warning.
.. tip:: Useful tip.
Specialized Text Blocks
Specialized text blocks like sidebars, code-blocks, and math expressions add depth to your documentation.
Sidebars: Use the .. sidebar:: directive to create a sidebar for supplementary information.
Code Blocks with Syntax Highlighting: For detailed code examples, use .. code-block:: language.
Math Expressions: Use .. math:: for embedding mathematical expressions and equations.

Advanced Formatting in reStructuredText
Advanced formatting in reStructuredText (reST) allows you to refine your documentation with nuanced styling and layout options. This section covers some of the more sophisticated features available in reST.
Inline Formatting
Bold and Italic Text: Emphasize key points or highlight important concepts by making text bold or italic.
Bold: Enclose text in double asterisks **bold text** to make it bold. Example: bold text
Italic: Enclose text in single asterisks *italic text* to italicize it. Example: italic text

Monospaced Text: Use monospaced font for code snippets, file paths, or any content where uniform character width is important.
Monospaced: Enclose text in double backticks `monospaced text`. Example: monospaced text

Inline Literals: Inline literals are useful for inserting code or command snippets within a paragraph.
Inline Code: Use double backticks for inline code `inline code`. Example: inline code

Subscript and Superscript
In scientific or mathematical documentation, you might need to use subscript and superscript.
Subscript: Use :sub: to create subscript text. Example: H\ :sub:2O (renders as H₂O).
Superscript: Use :sup: for superscript. Example: X\ :sup:2 (renders as X²).

Hyperlinks
Creating links is crucial in documentation to guide readers to additional resources or related topics.
External Links: Use angle brackets for URLs `OpenAI <https://www.openai.com>`_. Example: OpenAI
Internal Links: Reference other sections or documents with internal hyperlinks `See More <#target-section>`_.

Lets Practice
Start practicing by creating a simple document:
Open your chosen text editor and create a new file named practice.rst.
Write a short document:

Add a main heading and a few subheadings.
Include a paragraph under each heading.
Use Two elements 
Apply 2 advanced formatting 

3. Save your file and, if possible, generate a preview using Sphinx.
This initial practice will help you familiarize yourself with the basic syntax and flow of writing in reStructuredText.
Check if there is a way to share their previews
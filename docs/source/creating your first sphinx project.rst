Creating Your First Sphinx Project
==================================
We will focus on publishing your first index page and customizing the theme of your Sphinx documentation, using both Sphinx's built-in themes and the popular ReadTheDocs theme. This assumes you have already set up your Sphinx environment and are familiar with the basics of reStructuredText and Sphinx project structure.

Understanding the index.rst File
========================================

When you initialize a Sphinx project, an index.rst file is created by default. This file serves as the homepage or the root document of your documentation. The index.rst file typically contains a toctree directive, which is used to structure your documentation. We will talk more on this later

Customizing the index.rst File
==============================
(this is where you talk about using vs code and stuff)
Before diving into reStructuredText, ensure you have a suitable text editor. Any plain text editor will do, but those with markup language support (like VSCode, Sublime Text, or Atom) are recommended for their syntax highlighting and helpful features.


- Open the index.rst File: Locate and open this file in your preferred text editor or IDE.

- Add or modify the content. For example, introduce your project and provide an overview.

- Use the command sphinx-build html source html from your project's root directory. This command compiles your .rst files into HTML.

- Open the _build/html/index.html file in a web browser to see how your index.rst looks live.

How to Switch Themes in Sphinx
==============================
Sphinx supports numerous themes that can change your documentation's look and feel. Themes control the visual presentation of your content.

Sphinx Default Themes
------------------------------
- Find a Sphinx theme you like. You can browse through options here.

- In your conf.py file, find the html_theme variable and set it to the theme of your choice. For example:

html_theme = 'nature'

Run make html again to apply the new theme. Preview your changes by opening the newly built index.html.

ReadTheDocs Theme
------------------
The ReadTheDocs theme is widely appreciated for its clean, navigable layout and mobile-friendly design.

How to Install ReadTheDocs Theme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you haven't already, install the theme using pip:

pip install sphinx_rtd_theme

In your conf.py, set:

html_theme = 'sphinx_rtd_theme'

Run sphinx-build html source to apply the ReadTheDocs theme and then view your changes.




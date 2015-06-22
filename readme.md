JpGraph library for InfoRequest Bug Tracker
=============================
[![Logo](http://s6.postimg.org/b9hteq3m5/mantis_logo.png)](http://www.informatica-tr.com) - 
[![Build Status](https://travis-ci.org/FavioGalvis/Inforequest.svg?branch=modern-ui-2)](https://travis-ci.org/FavioGalvis/Inforequest) - 
[![Chat](http://s6.postimg.org/7f31s7l59/Screenshot_1.png)](http://webchat.freenode.net/?channels=%23inforequest&uio=OT10cnVlJjExPTIwNQa5)

For complete documentation, please read the guide on the jpgraph website,
The guide is available in text, PDF, and HTML formats.

Requirements
------------

 * Inforequest Alpha3 0.9
 * PHP 5.2+
 * a webserver (e.g. Apache or IIS)
 * Plugin Gráficos Mantis 1.3.0 Intalled

Installation
------------

 * Extract the tarball into the main folder location of your Inforequest installation
 * Point your browser to http://****/inforequest/manage_plugin_page.php to ensure that
   your plugins is compatible with Inforequest and configured correctly
 * Update de plugin configuration to *use jpgraph* in the plugin options
 * Update the config_ing.php file to include the root folder of the true type fonts
   add the line ---> $g_system_font_folder = 'truetype/';
 * Save
 * Installation is complete

UPGRADING
---------

 * Backup your existing installation and database -- really!
 * Extract the tarball into the main folder location of your Inforequest installation
 * Copy your configuration from the old installation to the new directory,
   including config_inc.php, custom_strings_inc.php, custom_relationships_inc.php,
   custom_functions_inc.php and custom_constants_inc.php if they exist
 * Upgrading is complete

CONFIGURATION
-------------

This file contains information to help you customize jpgraph.  A more
detailed doc can be found at http://jpgraph.net/download/manuals/

* There are several possible usage scenario for the library and it's different parts.

The most common usage is most likely to visualize numeric data by creating basic charts
(for example line, bar or pie charts) that is included dynamically in a WEB-page via
a straight forward <img> tag. The details on how to create dynamic graphs will be fully
covered in later sections of this manual The library itself is agnostic to where the
data comes from so it could for example be retrieved from a database, from a plain text
file or perhaps from some WEB-service. In addition to this scenario the library could be
used as a tool to create dynamic charts that are stored as image files in a directory.
This makes it possible to use the library in an off-line batch mode from the command line
(most likely using the cli =command line version of PHP).

* library/jpgraph.php - these files contains all the API library functions.

SCREENSHOTS
-------------
[![View.php](http://s6.postimg.org/b60rvtrgx/Screenshot_11.png)](http://www.informatica-tr.com)

Project-Jumper 0.1
==================

What is Project-Jumper?
-----------------------

Project Jumper is a Vim plugin which creates keyboard shortcuts for editing most common files or exploring most common directories. Currenty works only in Symfony 1.4 projects but I have plans to extend support to Symfony 2 and Rails 3.

Latest version
--------------

Latest version of Vim Project Jumper can be found at https://github.com/zergu/Vim-Project-Jumper

Installation
------------

Unpack all *.vim files and this README into ~/.vim/plugin/project-jumper/ directory. Restart Vim if necessary.

Usage
-----

Default shortucts work from Vim edit mode. To invoke a jump keep @ctrl@ presses and then type @j@ and other key depending whare you're trying to jump.

Shortcuts are working only when current directory (you can check it with :pwd command) is from inside a project. Avoid using shortucts elsewhere cause it can do some heavy and unsuccessful file searching.

Default shortcuts
-----------------

Project project related:
* <C-j><C-m> Model: Explore lib/model dir.
* <C-j><C-s> Schema: Edit config/*schema.yml (menu for multiple options).
* <C-j><C-y> CSS: Explore web/css dir.
* <C-j><C-j> JS: Explore web/js dir.
* <C-j><C-t> Test: Explore test dir.
* <C-j><C-h> Helper: Explore lib/helper dir.
* <C-j><C-f> Form: Explore lib/form dir.
* <C-j><C-i> Filter: Explore lib/filter dir.
* <C-j><C-l> Lib: Explore lib dir.
* <C-j><C-q> SQL: Explore data/sql dir.
* <C-j><C-x> Fixtures: Explore data/fixtures dir.

Application related (if your project has more that one application avaiable options are shown):
* <C-j><C-u> Layout: Edit $appname/templates/*layout*.php file (supports multiple options).
* <C-j><C-o> Modules: Explore $appname/modules dir.
* <C-j><C-r> Routing: Edit $appname/config/routing.yml file.
* <C-j><C-g> AppConfig: Edit $appname/config/app.yml file.
* <C-j><C-a> Action: Edit actions.class.php when editing or exploring module templates.
* <C-j><C-v> View: While cursor is placed on function header tries to edit associaded view. If none could be found, explores views directory.

Remapping shortucts
-------------------

Just copy mappings from the beginning of project-jumper.vim file to your .vimrc and modify it.
Skeleton Plugin for Joomla! 2.5+
================================

This repository is just a simple template to get you started creating a Joomla Plugin.

It includes all the base files and a languages folder with easily replaced "skeleton" placeholders to insert your own unique details and plugin name.

Getting started
---------------
Download the files ([zip][3]) or [fork][4] the repository.

####Replace Plugin Type and Name####
Make a copy of the files and using your favourite editor search and replace on the following to turn it into a starting point for your plugin.

- `plg-group` should be replaced by the plugins group (e.g. `content`)
- `GROUP` should be replaced by the plugins group<br />(note the all caps for language token keys is a Joomla style).
- `_skeleton` should be replaced by your plugins name<br />(usually something indicative of the functionality e.g. `embedtweet`)
- `_SKELETON` should also be replaced by your plugins name

[Plugin groups][1] are defined on the [Joomla Doc's website][2].

####Change File & Folder names####
For a plugin the top-level folder, and each of the files must follow a naming convention shown in the current file and folder structure:

	/skeleton/
		skeleton.php
		skeleton.xml
		languages/en-GB/en-GB.plg_plg-group_skeleton.ini
		languages/en-GB/en-GB.plg_plg-group_skeleton.sys.ini

Specifically, they must all match the name of the plugin in the XML file. That means where you find `plg-group` in a file name it must be replaced by the plugins group and where you find `skeleton` in a file name you should replace it with the name of your plugin.

So, for example if you have a `content` plugin with this name element in the XML `<name>plg_content_embedtweet</name>` the plugin file folder should be named:

	/embedtweet/
		embedtweet.php
		embedtweet.xml
		languages/en-GB/en-GB.plg_content_embedtweet.ini
		languages/en-GB/en-GB.plg_content_embedtweet.sys.ini


[1]: http://docs.joomla.org/Plugin/Events
[2]: http://docs.joomla.org
[3]: https://github.com/cppl/Skeleton-Plugin-for-Joomla/archive/master.zip
[4]: https://github.com/cppl/Skeleton-Plugin-for-Joomla/fork
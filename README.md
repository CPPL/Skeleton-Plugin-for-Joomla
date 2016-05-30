Skeleton Plugin for Joomla! 2.5+
================================

This repository is just a simple template to get you started creating a Joomla Plugin.

It includes all the base files and a languages folder with easily replaced "skeleton" placeholders to insert your own unique details and plugin name.

Getting started
---------------
Download the files ([zip][3]) or [fork][4] the repository.

#### Replace Plugin Type and Name####
Make a copy of the files and using your favourite editor do a **case sensitive** search and replace on the following to turn it into a starting point for your plugin.

_In this order:_

- `plg-group` should be replaced by the plugins group (e.g. `content`)
- `PLG-GROUP` should be replaced by the plugins group<br />(note the all caps for language token keys is a Joomla style).
- `Plg-Group` should be replaced by the plugins group (e.g. `Content`)<br />(note CamelCase for class/method names is a Joomla style).
- `_skeleton` should be replaced by your `_pluginName`<br />(usually something indicative of the functionality e.g. `_embedtweet`)
- Replace `skeleton` with your `pluginName`
    - `skeleton.php` with the name of your plugins main file e.g. `embedtweet.php`
    - `plugin="skeleton"` should change to `plugin="pluginName"` e.g. `plugin="embedtweet"`
- `_SKELETON` should also be replaced by your plugins name (e.g. `_EMBEDTWEET`)
- `Skeleton Plugin` with the human name of your plugin (e.g. `Embed Tweet Plugin`)
- `Skeleton` with class name of your plugin (e.g. `EmbedTweet`)
- `Copyright (C) YYYY Me or My Company` with your details e.g. `Copyright © 2015 Craig Phillips Pty Ltd`
- `My Name` with your name e.g. `Craig Phillips`
- `me@mydomain.com` with your email address (or support email address).
- `www.mydomain.com` with your website e.g. [www.craigphillips.biz](http://www.craigphillips.biz)
- `M YYYY` with the creation month and year e.g. `JULY 2015`

Finally do a case insensitive search for `skeleton` to find any remnants that may exist in sample text.

[Plugin groups][1] are defined on the [Joomla Doc's website][2].

#### Change File & Folder names####
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

### Annoyances
For Joomla 2.5.x+ in your plugins XML if you use a language key like `PLG_EMBEDTWEET_XML_DESCRIPTION` in the `<description>` element you must make sure that your package file (zip/gzip) doesn't include an extra folder level. To ensure your language files are loaded by the installer, files and directories of your plugin must be in the top-level of the zip file. For example for a packaged extension called `plg_content_embedtweet.zip` the structure should be like this:

```
plg_content_embedtweet.zip                      <-- the zip file
  embedtweet.php
  embedtweet.xml
  language/                                     <-- the language directory
    en-GB/                                      <-- the English language directory
      en-GB.plg_content_embedtweet.ini
      en-GB.plg_content_embedtweet.sys.ini
```

[1]: http://docs.joomla.org/Plugin/Events
[2]: http://docs.joomla.org
[3]: https://github.com/cppl/Skeleton-Plugin-for-Joomla/archive/master.zip
[4]: https://github.com/cppl/Skeleton-Plugin-for-Joomla/fork

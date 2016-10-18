# Slide-out Menu

This menu was written to be used on my personal website and across the accompanying subdomains ([camerondoyle.co.uk] (http://camerondoyle.co.uk)). A demonstration is available [here at camerondoyle.co.uk/menu-sample](http://camerondoyle.co.uk/menu-sample).

## Usage

This module is designed to be included as a submodule or subtree (your choice, I use it as a subtree) in a Jekyll project on GitHub pages. It's written entirely in HTML/CSS, and consists of a single file to allow an easy drop into your _includes folder.

To add this menu to your Jekyll project, take a fork of the project and run the following two commands from your project root folder:

    git remote add menu https://github.com/[your-github-username]/menu
    git subtree add --squash --prefix=_includes/menu/ menu template

This will include the 'template' branch in your Jekyll project. To call the menu, add the following line to any files in your _layouts folder that you want to apply them too (preferably immediately after your opening <body> tag):

    {% include menu/menu.html %}

By default, the menu includes four menu options. If you need to add or remove options, change the height value on line 16 (#scoped-slide-menu .side-menu-nav li) to [100 / $numberOfOptions].

## Bugs / Issues

Found an issue with this site? [Open a new issue here](https://github.com/CameronD17/menu/issues)

## Copyright and License

Copyright 2016 Cameron Doyle. Code released under the [Apache 2.0](https://github.com/CameronD17/menu/blob/gh-pages/LICENSE) license.
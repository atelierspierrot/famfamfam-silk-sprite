FamFamFam - Silk icons CSS sprite
=================================

The **UNOFFICIAL** sprites of the *FamFamFam Silk web icons*
by [FamFamFam](http://www.famfamfam.com).

**!! - This work is unofficial and is not liable for FamFamFam.**


## Overview

This package proposes a CSS sprite constructed on the
[FamFamFam Silk web-icons set](http://www.famfamfam.com/lab/icons/silk/).
The original set of icons is proposed under
[Creative Commons "Attribution" license](http://creativecommons.org/licenses/by/3.0/),
free of use as long as you attach image credits to
"[FamFamFam](http://www.famfamfam.com)".

To learn more about "CSS sprites" conception, see the
[Sprite (computer graphics) wikipedia's page](http://en.wikipedia.org/wiki/Sprite_%28computer_graphics%29#Sprites_by_CSS).


## Usage

### Installation

This package is a "standalone" CSS framework. To use it, you just need to get its sources
from GitHub and include the `src/` content of the package in your project assets.

If you are a [Bower](http://bower.io/) user, the package is registered so you can write
in your `bower.json`:

    "dependencies": {
        ...
        "atelierspierrot/famfamfam-silk-sprite": "dev-master"
    }

If you are a [Composer](http://getcomposer.org/) user, the package is referenced to 
Packagist so you can write in your `composer.json`:

    "require": {
        ...
        "atelierspierrot/famfamfam-silk-sprite": "dev-master"
    }

The package has a `library-assets` type to allow handling by the
[Assets Manager](http://github.com/atelierspierrot/assets-manager) Composer's extension. If
you plan to use the manager, you can use the `assets-install` branch of the package, which
has the AssetsManager in its requirements (to be sure it will be loaded before the sprite
and be able to move it in the project assets).

### HTML usage

Once the package is included in your project, you can start to use the sprites framework.

To do so, you first need to include the CSS definitions:

	<link rel="stylesheet" href="path/to/package/src/silk-icons-sprite.min.css" />

Then you can start writing some Silk icons spans using the framework explained below.

A demonstration page is available in the global package in `demo/` ; it shows in particular
the list of available icons and their names.

### CSS Framework

The package defines some **CSS sprite** classes to render some icons easily and with
least of work.

The CSS framework to use the sprites is based on two classes:

-   the first one that is common and global: `web-icon`,
-   the last one to choose the icon itself, which is the name of the icon.

For instance, to render a the "print" icon, you will write:

    <span class="web-icon print"></span>

As the sprite is not defined with restrictive CSS rules, you may encounter rendering
problems (such as margins or paddings defined globally in your document) that can be avoid
adding a `reset` class to your icons:

    <span class="web-icon reset print"></span>


## Credits

As mentioned above, the original set of icons is made by [FamFamFam](http://www.famfamfam.com/)
(Mark James - UK) and proposed under [Creative Commons Attribution](http://creativecommons.org/licenses/by/3.0/)
license. You are free to use it in any work but you must always add
a link to www.famfamfam.com in a prominent place (e.g. the page footer), including the
CC-BY license and the reference to www.famfamfam.com on every page using the icons.

The sprite was generated with the help of [website-performance.org](http://spritegen.website-performance.org/)
and is CSS3 valid.

The minified version of the CSS file of the package was processed with the [YUI Compressor](http://refresh-sf.com/yui/).

The PNG sprite is optimized using [Smush.it (TM)](http://www.smushit.com/ysmush.it/).

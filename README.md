# Starter Kit

The Predix Experience Starter Kit is one of Px's meta kits and simply ties together a few key dependencies that are usually the starting point for any new project. It is a fork of inuitcss' [starter-kit](https://github.com/inuitcss/starter-kit). The Starter Kit specifically contains Px and inuitcss default variables and mixins, as well as [Nicolas Gallagher](https://twitter.com/necolas)’s [Normalize.css](https://github.com/necolas/normalize.css), global `box-sizing`, viewport, and typography rules.

Additionally, the Starter Kit includes unobtrusive helper and trump classes for use within a project. This enables by default utilities to help with responsive implementation and micro spacing strategies.

## Dependencies

Strictly speaking, the Starter Kit is just a collection of dependencies and nothing else. There is no Sass file, just modules you can import into your project as a starting point.

## Installation

    $ bower install --save https://github.build.ge.com/PXd/px-starter-kit-design.git

## Usage

The modules must be imported in the following order:

    // Generic
    @import "px-normalize-design/_generic.normalize.scss";
    @import "px-box-sizing-design/_generic.box-sizing.scss";
    @import "px-helpers-design/_generic.helpers.scss";
    
    // Base
    @import "px-flexbox-design/_base.flexbox.scss";
    @import "px-viewport-design/_base.viewport.scss";
    @import "px-typography-design/_base.typography.scss";
    
    // Trumps
    @import "inuit-clearfix/_trumps.clearfix.scss";
    @import "px-spacing-responsive-design/_trumps.spacing-responsive.scss";
    @import "px-widths-responsive-design/_trumps.widths-responsive.scss";

## NPM & Grunt

Also, the Starter Kit includes `package.json` and `Gruntfile.js` templates (as well as the necessary supporting grunt task configurations) for compiling your Sass and passing the resulting CSS through [Autoprefixer](https://github.com/postcss/autoprefixer).

To get these, `git clone` this repository. Note, you'll need to fill in paths relevant to your project in the grunt tasks (found under `tasks/options`) replacing `'TODO'`.

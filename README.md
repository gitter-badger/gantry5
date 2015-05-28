Gantry Framework
================

[![Join the chat at https://gitter.im/adi8i/gantry5](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/adi8i/gantry5?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Join the chat at https://gitter.im/gantry/gantry5](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/gantry/gantry5?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Ready to get started with Gantry 5? That's great! We are here to help.

On this page, you will get some quick tips to help you hit the ground running with Gantry 5. You can find more detailed documentation for each of these tips by clicking the **Learn More** button at the bottom of each section.

We hope you enjoy Gantry 5 every bit as much as we have enjoyed making it.

## Browser Requirements

The back-end administration requirements of Gantry in order of preference are as follows:

* Google Chrome 41+
* Firefox 36+
* Safari 8+
* Opera 28+
* Internet Explorer 10+ (9 supported at limited capacity)

## Installing Gantry 5 and the Hydrogen Theme

Gantry 5 is a framework by which Gantry-powered themes are made. In order for a Gantry theme to work, you will need to install both the **framework** and the **theme**. Doing this is not difficult at all.

The first thing you need to do is download the latest build of Gantry 5 and Hydrogen. You can do so by clicking the links below, or via [GitHub](http://github.com/gantry/gantry5/).

* [Download Gantry 5](https://github.com/gantry/gantry5/releases/download/5.0.0-rc.2/joomla-pkg_gantry5_v5.0.0-rc.2.zip)
* [Download Hydrogen Theme](https://github.com/gantry/gantry5/releases/download/5.0.0-rc.2/joomla-tpl_g5_hydrogen_v5.0.0-rc.2.zip)

>>> During the initial beta, the **Framework** and **Template** are being distributed in different installable packages. A bundled package is planned, but will likely be available after the initial beta launch.

Once you have the latest packages, installation is simple. We have provided a step-by-step guide in the **Installation** portion of this documentation.

[**Learn More**](http://docs.gantry.org/gantry5/basics/installation)

## Accessing the Gantry Administrator

### Joomla
When you have installed and activated both the Gantry framework and Hydrogen, you can access the Gantry 5 administrator in several different ways. The easiest being simply navigating to **Components > Gantry 5 Templates** from the back end of Joomla.

Here, you will see a list of any installed Gantry-powered themes. You can **Preview** the theme from here or select **Configure** to go directly to the **Gantry Administrator** where you can get started modifying your Gantry-powered site.

## Navigating the Gantry 5 Administrator

The Gantry Administrator has multiple administrative tools you can flip through to configure how your Gantry-powered theme looks and functions. Here is a quick breakdown of each of these tools, and what you can do with them.

You will notice the following menu items in the Gantry 5 Administrator:

1. **Menu Editor**: This administrative panel gives you the ability to enhance the platform's menu by altering styling, rearranging links, and creating menu items that sit outside of the CMS's integrated Menu Manager.

2. **About**: This page gives you quick, at-a-glance information about the currently-accessed theme. This is a one-stop shop for information about the theme including: name, version number, creator, support links, features, and more.

3. **Platform Settings**: This button takes you to the CMS' settings page for Gantry 5. In Joomla, this is the **Permissions** configuration page.

4. **Clear Cache**: This button clears the cache files related to Gantry. This includes all of the temporary files outside of CSS and configuration information.

5. **Configuration Dropdown**: This dropdown makes it easy to quickly switch between Configurations without having to leave the Gantry Administrator.

6. **Styles**: This administrative panel gives you access to style related configuration settings. This includes things like theme colors, fonts, style presets, and more.

7. **Settings**: This administrative panel offers you the ability to configure the functional settings of the theme. This includes setting defaults for Particles, as well as enabling/disabling individual Particles.

8. **Layout**: This administrative panel is where you would configure the layout for your theme. Creating an placing module positions, Particles, spacers, and non-rendered scripts such as Google Analytics code is all done in this panel.

[**Learn More**](http://docs.gantry.org/gantry5/configure/gantry-admin)

## What are Configurations, Particles, Atoms, etc.?

Because Gantry 5 is so different from any version of Gantry before it, we came up with some terms to help make sense of the relationships Gantry's new features have with one-another. Here is a quick breakdown of commonly used terms related to Gantry 5.

| Term          | Definition                                                                                                                                             |
| :-----        | :-----                                                                                                                                                 |
| Configuration | A configurable style used in one or more areas of your site. It serves as the container on which a page's style, settings, and layout are set.         |
| Particle      | A typically small block of data used on the front end. It acts a lot like a widget/module, but can be easily configured in the Gantry 5 Administrator. |
| Atom          | A type of Particle that contains non-rendered data, such as custom scripting (JS, CSS, etc.) or analytics scripts for traffic tracking.                |

[**Learn More**](http://docs.gantry.org/gantry5/basics/terminology)

## Where to Get Help

A chat room has been set up using [Gitter](https://gitter.im/gantry/gantry5) where you can go to talk about the project with developers, contributors, and other members of the community. This is the best place to go to get quick tips and discuss features with others.

[Documentation](http://docs.gantry.org) is also available, and being continually added to as development progresses. Is something missing? You can contribute to the documentation through GitHub.

## How to Contribute

Contributing to the Gantry 5 framework, or to its associated documentation is easy. Development for both of these projects is being conducted via [Github](http://github.com), where you can submit **Issues** to report any bugs or suggest improvements, as well as submit your own **Pull Requests** to submit your own fixes and additions.

We recommend chatting with the team via [Gitter](https://gitter.im/gantry/gantry5) prior to submitting the pull request to avoid doubling up on a fix that is already pending or likely to be overwritten by an upcoming change.

## Bundling JS and Compiling SCSS

In our development environment, we use **Gulp** to bundle **JavaScript** and compile **SCSS** with the capability of `watch` so that any change on target files will automatically trigger the recompilation.

If you would like to set this up in your own development environment, you can do so following these simple instructions.

> Note that for this to work, you need to have **Gantry 5** source and not a package. You can either **clone** it or **download** the source from GitHub.

The first thing you need is `Node / NPM`. If you don’t have them already, you can grab the installer for your OS from [https://nodejs.org/download/](https://nodejs.org/download/).

Once that’s done, you can install **Gulp**. We recommend installing Gulp globally so you can use the command from any folder. Here is the command to do so: `npm install —-global gulp`

Now that you have the required pieces, the next step is to install all of the JS module dependencies. To do so, make sure you are at the root of the Gantry 5 project, and run the command `npm install`.

Because we have two sets of JS applications, one for admin and one for the site, you will also need to install the JS modules for those. Still, from the root of your project you can run this command:

`cd platforms/common/ && npm install && cd ../../assets/common/ && npm install && cd ../../`

At this point you have everything you need to run Gulp. Just type the command `gulp` and you should see the CSS and JS getting compiled.

We provide a few handy tasks as well:

  1. `$ gulp` / `$ gulp all`: Compiles all of the CSS and JS in the project.
  2. `$ gulp watch`: Starts the compilers in `watch` mode. Any change applied to targeted **JS** or **SCSS** files will trigger an automatic recompilation.
  3. `$ gulp css` / `$ gulp js`: Compiles all of either CSS or JS files, in case you are only working on one and not the other.
  4. `$ gulp —prod`: Compiles every CSS and JS in production mode. The compiled files won’t have source maps and will be compressed (this usually takes slightly longer than normal mode).

Symfony Quick Start
========================

## What is it?

This is the [Symfony3 Standard Edition](https://github.com/symfony/symfony-standard) with some ready-to-use tools to get started quickly.

Most common stuff, translations or menus are built-in: no need to configure or code anything. Just overwrite and copy/paste to customize.

This lite version doesn't contain any login feature, nor database requirement.

You'll find here 2 bundles:

- Fuz\QuickStartBundle contains well-known bundles implementations, you'll probably not need to modify those files.

- AppBundle is a skeleton, it will contain your app implementation.

## Ready-to-use bundles

- BootstrapBundle is preinstalled with a base layout, and will automatically render your forms the right way, and display flash messages using the right color.

- i18n support with language switcher and specific routes for each supported locales.

- KnpMenu awaits your routes and labels as an associative array for logged and non-logged users in a single class; it is already implemented at the top of the base layout.

- Project already implements 403, 404, 500 and generic error pages, no need to worry about the common pitfalls on the subject.

- CRUD generator generates bootstrap-ready and translated views, because if you need this app, you're not against generating most of the application.

- CKeditor and HTMLPurifier are preinstalled to manage rich-text editors (WYSIWYG), just use CKEditorType in your form and |purify filter in your view.

## Installation

```sh
php -r "readfile('https://getcomposer.org/installer');" | php
php composer.phar update
php app/console assets:install web --symlink
```

## Usage

Most of the features can be configured or disabled inside the `parameters.yml` configuration file.

## License

- This project is released under the MIT license

- Fuz logo is © 2013-2016 Alain Tiemblo


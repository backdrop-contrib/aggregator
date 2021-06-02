Aggregator
======================

Aggregate RSS feeds and publish them in a River of News format. To add
blocks, use the Views module, for which a plugin is provided.

Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

- Visit the configuration page under Administration > Configuration >
  Web services > Feed aggregator (admin/config/services/aggregator) to
  add feeds and categories.

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

SSL Verification
----------------

If a feed's URL fails SSL verification, a setting is available to disable it.

For example:

```
The feed from ___ seems to be broken, due to "0 Error opening socket ssl://___:443".
```

To disable SSL verification, set it through [Drush](https://github.com/backdrop-contrib/backdrop-drush-extension):

```
drush config-set aggregator.settings aggregator_ssl_verification 0
```

There is currently no UI for this setting. This is a global setting, meaning
it applies to all feeds, so it should be turned off with forethought.

Current Maintainers
-------------------

- Richard Eriksson (https://github.com/sillygwailo)

Credits
-------

This module was originally developed by the Drupal community for the core
Drupal project.
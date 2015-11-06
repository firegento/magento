# Magento Community Edition

Firegento Magento Community Magento-1.x Mirror Github Repository with Patches.

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/firegento/magento?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

- [available magento versions](https://github.com/firegento/magento/releases)
- [an overview of all patches](https://github.com/brentwpeterson/magento-patches)

## Installation via Composer

If you do not know what Composer is, please first read [this](https://getcomposer.org/doc/00-intro.md).

Your main root project `composer.json` file can look like this:

```json
{
    "repositories": {
        "firegento": {
          "type": "composer",
          "url": "http://packages.firegento.com"
        }
    },
    "require": {
      "magento-hackathon/magento-composer-installer": "~3.0",
      "aydin-hassan/magento-core-composer-installer": "~1.2",
      "firegento/magento": "~1.9.2"
    },
    "extra": {
      "magento-root-dir": "src",
      "auto-append-gitignore": true,
      "magento-deploystrategy": "copy",
      "magento-force": true
    }
}
```

To install magento:

* create webroot `src`
* run `composer install`

To update magento:

* run `composer update`

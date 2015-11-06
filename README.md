Magento Community Edition
==========

Magento Community Edition

- [1.7.0.2](https://github.com/firegento/magento/tree/v1.7.0.2)
- [1.7.0.2+patch1](https://github.com/firegento/magento/tree/v1.7.0.2+patch1) (unoffical)
- [1.8.1.0](https://github.com/firegento/magento/tree/v1.8.1.0)
- [1.8.1.0+patch1](https://github.com/firegento/magento/tree/v1.8.1.0+patch1) (unoffical)
- [1.8.1.0+patch2](https://github.com/firegento/magento/tree/v1.8.1.0+patch2) (unoffical)
- [1.9.0.0](https://github.com/firegento/magento/tree/v1.9.0.0)
- [1.9.0.1](https://github.com/firegento/magento/tree/v1.9.0.1)
- [1.9.0.1+patch1+SUPEE-6788](https://github.com/firegento/magento/tree/v1.9.0.1+patch1+SUPEE-6788)
- [1.9.1.0](https://github.com/firegento/magento/tree/v1.9.1.0)
- [1.9.1.1](https://github.com/firegento/magento/tree/v1.9.1.1)
- [1.9.1.1+patch1](https://github.com/firegento/magento/tree/v1.9.1.1+patch1) (unoffical)
- [1.9.1.1+patch2](https://github.com/firegento/magento/tree/v1.9.1.1+patch2) (unoffical)
- [1.9.2.0](https://github.com/firegento/magento/tree/1.9.2.0)
- [1.9.2.1](https://github.com/firegento/magento/tree/1.9.2.1)
- [1.9.2.2](https://github.com/firegento/magento/tree/v1.9.2.2)

[https://www.magentocommerce.com/products/downloads/magento/](https://www.magentocommerce.com/products/downloads/magento/)

### 1.9.2.2

- Includes patches: SUPEE-5344, SUPEE-5994, SUPEE-6237, SUPEE-6285, SUPEE-6482, SUPEE-6788

### 1.9.2.1

- Includes patches: SUPEE-5344, SUPEE-5994, SUPEE-6237, SUPEE-6285, SUPEE-6482 

### 1.9.1.1+patch2

- PATCH_SUPEE-5994_EE_1.14.1.0_v1-2015-05-14-05-05-02.sh

### 1.9.1.1+patch1

- PATCH_SUPEE-5344_CE_1.8.0.0_v1-2015-02-10-08-10-38.sh
- PATCH_SUPEE-4829_EE_1.14.1.0_v1-2015-02-10-07-57-21.sh

### v1.9.1.1

Contains SUPEE-5344

### v1.9.0.0 + v1.9.0.1 + v1.9.1.0 + v1.9.0.1+patch1+SUPEE-6788

Insecure, do not use!

### v1.8.1.0+patch2

- PATCH_SUPEE-5994_EE_1.14.1.0_v1-2015-05-14-05-05-02.sh

### v1.8.1.0+patch1

- PATCH_SUPEE-1049_EE-1.12.0.2_v1.sh
- PATCH_SUPEE-2747_EE_1.13.1.0_v1.sh
- PATCH_SUPEE-5344_CE_1.8.0.0_v1.sh
- PATCH_SUPEE-1533_EE_1.13.x_v1.sh
- PATCH_SUPEE-3941_EE_1.14.0.1_v1.sh
- PATCH_SUPEE-1868_EE_1.13.x_v1.sh *USPS NOT APPLIED, conflict*
- PATCH_SUPEE-4334_EE_1.11.0.0-1.13.0.2_v1.sh *USPS NOT APPLIED, conflict*

### v1.8.1.0

Insecure, do not use!

### 1.7.0.2+patch1

- PATCH_SUPEE-5994_EE_1.14.1.0_v1-2015-05-14-05-05-02.sh

### v1.7.0.2

Insecure, do not use!

### All patches CE+EE

An overview of all patches can be found here: [https://github.com/brentwpeterson/magento-patches](https://github.com/brentwpeterson/magento-patches)

## Installation via Composer

If you do not know what Composer is, please first read [this](https://getcomposer.org/doc/00-intro.md).

You main root project composer.json file can look like this:

```json
{
    "repositories": {
        "magento": {
          "type":"git", 
          "url":"https://github.com/firegento/magento"
        },
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

* create webroot src
* run `composer install`

To update magento:

* run `composer update`

Magento Community Edition
==========

Magento Community Edition

- [1.7.0.2](https://github.com/firegento/magento/tree/v1.7.0.2)
- [1.7.0.2+patch1](https://github.com/firegento/magento/tree/v1.7.0.2+patch1) (inoffical)
- [1.8.1.0](https://github.com/firegento/magento/tree/v1.8.1.0)
- [1.8.1.0+patch1](https://github.com/firegento/magento/tree/v1.8.1.0+patch1) (inoffical)
- [1.8.1.0+patch2](https://github.com/firegento/magento/tree/v1.8.1.0+patch2) (inoffical)
- [1.9.0.0](https://github.com/firegento/magento/tree/v1.9.0.0)
- [1.9.0.1](https://github.com/firegento/magento/tree/v1.9.0.1)
- [1.9.1.0](https://github.com/firegento/magento/tree/v1.9.1.0)
- [1.9.1.1](https://github.com/firegento/magento/tree/v1.9.1.1)
- [1.9.1.1+patch1](https://github.com/firegento/magento/tree/v1.9.1.1+patch1) (inoffical)
- [1.9.1.1+patch2](https://github.com/firegento/magento/tree/v1.9.1.1+patch2) (inoffical)

[https://www.magentocommerce.com/products/downloads/magento/](https://www.magentocommerce.com/products/downloads/magento/)

### 1.9.1.1+patch2

- PATCH_SUPEE-5994_EE_1.14.1.0_v1-2015-05-14-05-05-02.sh

### 1.9.1.1+patch1

- PATCH_SUPEE-5344_CE_1.8.0.0_v1-2015-02-10-08-10-38.sh
- PATCH_SUPEE-4829_EE_1.14.1.0_v1-2015-02-10-07-57-21.sh

### v1.9.1.1

Contains SUPEE-5344

### v1.9.0.0 + v1.9.0.1 + v1.9.1.0

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
    "name": "myCompany/myOnlineStore"
    "description": "The ACME Online Store!",
    "license": "OSL-3.0",
    "authors": [
        {
            "name": "Road Runner",
            "email": "meepmeep@acme.com"
        }
    ],
    "require": {
        "firegento/magento": "1.9.1.1+patch2",
    },
    "scripts": {
        "post-install-cmd": [
            "cp -R vendor/magento/magento/* path/To/My/Magento/Root/Directory/"
        ],
        "post-update-cmd": [
            "cp -R vendor/magento/magento/* path/To/My/Magento/Root/Directory/"
        ]
    },
}
```

To run it: 

```
composer.phar install -vv
```

This will download the version `1.9.1.1+patch2` from GitHub, 
unzips it and places the files in the folder `vendor/magento/magento`. 

A post install/update script copies those files to your root folder. 
If you want to update to the next version simply replace `1.9.1.1+patch2` with the next version. 

There are typos in the above JSON to prevent you from blind copying. 
If you think this feels wrong please suggest an alternative way via an issue.

### Tags

All tags are signed with my *Cyrill AT Schumacher dot fm* [PGP key](http://www.schumacher.fm/cyrill.asc).

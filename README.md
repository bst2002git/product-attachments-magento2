[![Latest Stable Version](https://poser.pugx.org/lizardmedia/module-product-attachments/v/stable)](https://packagist.org/packages/lizardmedia/module-product-attachments)
[![Total Downloads](https://poser.pugx.org/lizardmedia/module-product-attachments/downloads)](https://packagist.org/packages/lizardmedia/module-product-attachments)
[![License](https://poser.pugx.org/lizardmedia/module-product-attachments/license)](https://packagist.org/packages/lizardmedia/module-product-attachments)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/lizardmedia/product-attachments-magento2/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/lizardmedia/product-attachments-magento2/?branch=master)
[![Build Status](https://scrutinizer-ci.com/g/lizardmedia/product-attachments-magento2/badges/build.png?b=master)](https://scrutinizer-ci.com/g/lizardmedia/product-attachments-magento2/build-status/master)

# Magento 2 Product Attachments

Module `LizardMedia_ProductAttachment` adds possibility to add attachment for products.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

* Magento 2.2
* PHP 7.1

### Installing

#### Download the module

##### Using composer (suggested)

Simply run

```
composer require lizardmedia/module-product-attachments
```

##### Downloading ZIP

Download a ZIP version of the module and unpack it into your project into
```
app/code/LizardMedia/ProductAttachment
```

#### Install the module

Run this command
```
bin/magento module:enable LizardMedia_ProductAttachment
bin/magento setup:upgrade
```

## Usage

#### Admin panel

* add and manage attachments to product via adminhtml form

#### Frontend
* display attachments on product view page
* display attachments in customer account bookmark

## For developers

In case of uploading bigger files may be necessary adjusting some configuration with higher values:
* nginx - `client_max_body_size`
* php - `memory_limit` && `upload_max_filesize` && `post_max_size`

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/lizardmedia/varnish-warmer-magento2/tags).

## Authors

* **Bartosz Kubicki** - *Initial work* - [Lizard Media](https://github.com/bartek9007)

See also the list of [contributors](https://github.com/lizardmedia/product-attachments-magento2/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## To do

* Introduce EAV pattern for attachment entity to make it vary depending on store view id
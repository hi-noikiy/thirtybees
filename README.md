# thirty bees 
[![Build Status](https://travis-ci.org/thirtybees/thirtybees.svg?branch=master)](https://travis-ci.org/thirtybees/thirtybees)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/thirtybees/thirtybees/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/thirtybees/thirtybees/?branch=master)
[![Crowdin](https://d322cqt584bo4o.cloudfront.net/thirty-bees/localized.svg)](https://crowdin.com/project/thirty-bees)
[![Gitter](https://img.shields.io/gitter/room/thirtybees/General.svg)](https://gitter.im/thirtybees/General)

thirty bees is an open-source fork of PrestaShop 1.6. Our aim with this fork is to provide a feature set that merchants need. We are rewriting a lot of the core modules and cleaning up the legacy code. We aim to provide a stable, feature-rich e-commerce platform to grow businesses.  

![thirty bees screenshot](https://cloud.githubusercontent.com/assets/6775736/22063185/c5ef8e3c-dd7d-11e6-923c-4b62ac404c86.png)


## Roadmap for thirty bees version 1.1.x

**New Features being added into v1.1.x of thirty bees:**

No ideas, yet. Would you mind helping us with that? https://thirtybees.com/feature-request/

### Updated roadmap
You can find the latest version of the roadmap here: https://thirtybees.com/roadmap

## Requirements
**General server requirements:**

- PHP 5.6 - PHP 7.1
- Apache, nginx or IIS
- Windows, Linux or OS X
- MySQL 5.5.3+ or MariaDB 5.5+
- PHP extensions:
  - Required:
    - gd
    - bcmath
    - xml (SimpleXML, DOMDocument)
    - json
    - zip
    - mysql (PDO only)
    - mbstring
  - Recommended:
    - imap
    - curl
    - opcache
    - apcu/redis/memcache(d)

## Installation
You can install the master or follow a [release package](https://github.com/thirtybees/thirtybees/releases) 
- Recursively clone the repository and choose tag release version number from the -b parameter:
```shell
$ git clone https://github.com/thirtybees/thirtybees.git --recursive -b #.##
```
- Then cd into the `thirtybees` folder
- Run composer to install the dependencies:
```shell
$ composer install
```
- Then install the software as usual, using either a web browser (https://example.com/install-dev) 
- Or install via command line 
``` php /install-dev/index_cli.php```
    - Arguments available:
```
--step          all / database,fixtures,theme,modules,addons_modules    (Default: all)
--language      Language iso code                                       (Default: en)
--all_languages Install all available languages                         (Default: 0)
--timezone                                                              (Default: Europe/Paris)
--base_uri                                                              (Default: /)
--domain                                                                (Default: localhost)
--db_server                                                             (Default: localhost)
--db_user                                                               (Default: root)
--db_password                                                           (Default: )
--db_name                                                               (Default: thirtybees)
--db_clear      Drop existing tables                                    (Default: 1)
--db_create     Create the database if not exist                        (Default: 0)
--prefix                                                                (Default: tb_)
--engine        InnoDB                                                  (Default: InnoDB)
--name                                                                  (Default: thirty bees)
--activity                                                              (Default: 0)
--country                                                               (Default: fr)
--firstname                                                             (Default: John)
--lastname                                                              (Default: Doe)
--password                                                              (Default: 0123456789)
--email                                                                 (Default: pub@thirtybees.com)
--license       Show thirty bees license                                (Default: 0)
--newsletter    Get news from thirty bees                               (Default: 1)
--send_email    Send an email to the administrator after installation   (Default: 1)
```

## Contributing
See [CONTRIBUTING.md](CONTRIBUTING.md)

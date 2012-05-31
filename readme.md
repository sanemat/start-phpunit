$ mkdir -p start-phpunit
$ cd start-phpunit
$ curl -s http://getcomposer.org/installer | ~/lib/php54/bin/php
#!/usr/bin/env php
All settings correct for using Composer
Downloading...

Composer successfully installed to: /Users/sane/work/php-study/start-phpunit/composer.phar
Use it: php composer.phar

$ git init
Initialized empty Git repository in /Users/sane/work/php-study/start-phpunit/.git/
$ touch .gitkeep
$ git add .gitkeep
$ git commit -v

$ /Users/sane/lib/php54/bin/php composer.phar init

                                            
  Welcome to the Composer config generator  
                                            


This command will guide you through creating your composer.json config.

Package name (<vendor>/<name>) [sanemat/start-phpunit]:
Description []: How to start project with phpunit.
Author [sanemat <o.gata.ken@gmail.com>]:

Define your dependencies.

Would you like to define your dependencies (require) interactively [yes]?
Search for a package []: phpunit

Found 9 packages matching phpunit

   [0] EHER/PHPUnit 1.3
   [1] EHER/PHPUnit 1.4
   [2] EHER/PHPUnit 1.1
   [3] EHER/PHPUnit 1.2
   [4] EHER/PHPUnit 1.5
   [5] EHER/PHPUnit 1.6
   [6] EHER/PHPUnit dev-composer
   [7] EHER/PHPUnit dev-master
   [8] benmatselby/phpunit-testlistener-mongo dev-master

Enter package # to add, or a "[package] [version]" couple if it is not listed []: 5
Would you like to define your dev dependencies (require-dev) interactively [yes]?
Search for a package []:

{   
    "name": "sanemat/start-phpunit",
    "description": "How to start project with phpunit.",
    "require": {
        "eher/phpunit": "1.6"
    },
    "authors": [
        {   
            "name": "sanemat",
            "email": "o.gata.ken@gmail.com"
        }
    ]
}

Do you confirm generation [yes]?
Would you like the vendor directory added to your .gitignore [yes]?
s
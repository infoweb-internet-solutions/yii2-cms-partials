CMS partials module for Yii 2
========================

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require infoweb-internet-solutions/yii2-cms-partials "*"
```

or add

```
"infoweb-internet-solutions/yii2-cms-partials": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply modify your backend configuration as follows:

```php
return [
    ...
    'modules' => [
        'partials' => [
            'class' => 'infoweb\partials\Module',
        ],
    ],
    ...
];
```

Import the translations and use category 'infoweb/partials':
```
yii i18n/import @infoweb/partials/messages
```

To use the module, execute yii migration
```
yii migrate/up --migrationPath=@vendor/infoweb-internet-solutions/yii2-cms-partials/migrations
```

## Requirements

This plugins has been developped for cakephp 3.x.

## Installation

You can install this plugin into your CakePHP application using [composer](http://getcomposer.org).

Update your composer file to include this plugin:

```
composer require oxenti/soft-delete
```

## Configuration

1. Load the plugin:

```
// In /config/bootstrap.php
Plugin::load('SoftDelete');
```

2. Make a model soft deleteable by using SoftDelete trait:

```
// in src/Model/Table/UsersTable.php
...
use SoftDelete\Model\Table\SoftDeleteTrait;

class UsersTable extends Table
{
    use SoftDeleteTrait;
    ...
```

## WordPress database prefixer

Simple utility class to rename a site's database prefix. This is a modified copy of [https://github.com/iandunn/wp-cli-rename-db-prefix](https://github.com/iandunn/wp-cli-rename-db-prefix) so that it is not restricted to WP CLI usage only.

Please note this is not compatible with a multisite setup.

### Install

```
composer require pressmodo/database-prefixer
```

### Usage

```php
use Pressmodo\DB\DatabasePrefixer;

$run = ( new DatabasePrefixer( $newPrefix ) )->init();
```
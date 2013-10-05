# Airbrake Silex Extension

[Airbrake][1] service provider for [Silex][2] and [php-airbrake][3].

## Installation

composer.json:

```json
{
    "require": {
      "dbtlr/php-airbrake"    : "dev-master",
      "merqlove/airbrake-silex-service-provider"    : "dev-master"
    }
}
```

```bash
$ wget http://getcomposer.org/composer.phar
$ php composer.phar install
```

## Registering

```php
use Merqlove\Silex\Provider\AirbrakeServiceProvider;

$app->register(new AirbrakeServiceProvider(), array(
    'airbrake.api_key' => 'SOME_KEY', //required
    'airbrake.options' => array(
      'secure' => false,
    ), // optional
));
```

## License

The Airbrake Silex Extension is licensed under the MIT license.

[1]: https://airbrake.io
[2]: http://silex-project.org
[3]: https://github.com/dbtlr/php-airbrake

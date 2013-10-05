# Airbrake Silex Extension

Airbrake service provider for [Silex][1] and [php-airbrake][2].

## Installation

composer.json:

```json
{
    "require": {
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

## Credits

* [Airbrake][3]

## License

The Airbrake Silex Extension is licensed under the MIT license.

[1]: http://silex-project.org
[2]: https://airbrake.io
[3]: https://github.com/dbtlr/php-airbrake

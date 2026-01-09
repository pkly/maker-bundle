# Contributing

This project is part of the Symfony ecosystem and follows the
[Symfony Contribution Guidelines](https://symfony.com/doc/current/contributing/index.html).

## Running Tests

This project uses [PHPUnit Bridge](https://phpunit.de/getting-started/phpunit-bridge.html) to run the tests.

Install the required dependencies with:

```bash
composer install
```

To run the tests, use the following command:

```bash
./vendor/bin/simple-phpunit
```

## Static Analysis

This project uses [PHPStan](https://phpstan.org/) for static analysis.
To run PHPStan, use the following command:

Install the required dependencies for the project, PHPStan itself and the extra
packages that the project uses:

```bash
composer update
composer update --working-dir=tools/phpstan
composer update --working-dir=tools/phpstan/includes
```

Run PHPStan with:

```bash
tools/phpstan/vendor/bin/phpstan
```

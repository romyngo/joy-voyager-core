# Joy VoyagerCore

This [Laravel](https://laravel.com/)/[Voyager](https://voyager.devdojo.com/) module adds VoyagerCore support to Voyager.

By 🐼 [Ramakant Gangwar](https://github.com/rxcod9).

[![Screenshot](https://raw.githubusercontent.com/rxcod9/joy-voyager-core/main/cover.jpg)](https://joy-voyager.kodmonk.com)

[![Latest Version](https://img.shields.io/github/v/release/rxcod9/joy-voyager-core?style=flat-square)](https://github.com/rxcod9/joy-voyager-core/releases)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rxcod9/joy-voyager-core/run-tests.yml?branch=main&label=tests)
[![Total Downloads](https://img.shields.io/packagist/dt/joy/voyager-core.svg?style=flat-square)](https://packagist.org/packages/joy/voyager-core)

---

## Prerequisites

*   Composer Installed
*   [Install Laravel](https://laravel.com/docs/installation)
*   [Install Voyager](https://github.com/romyngo/voyager)

---

## Installation

This fork is not published on Packagist, so add the fork repositories to your Laravel project's `composer.json` first (repositories declared inside a dependency are ignored, so all three must be listed here):

```json
"repositories": {
    "voyager-core": { "type": "vcs", "url": "https://github.com/romyngo/joy-voyager-core" },
    "voyager": { "type": "vcs", "url": "https://github.com/romyngo/voyager" },
    "joy-core": { "type": "vcs", "url": "https://github.com/romyngo/joy-core" }
}
```

The `joy-core` repository hosts the `romyngo/core` package (its `composer.json` name), the fork of [rxcod9/joy-core](https://github.com/rxcod9/joy-core).

```bash
# 1. Require this Package in your fresh Laravel/Voyager project
composer require romyngo/voyager-core:dev-master

# 2. Publish
php artisan vendor:publish --provider="Joy\VoyagerCore\VoyagerCoreServiceProvider" --force

# 3. Publish voyager overriden views [MANDATORY]
php artisan vendor:publish --provider="Joy\VoyagerCore\VoyagerCoreServiceProvider" --tag="overwrite-voyager-views" --force
```

---

<!-- ## Usage

Installation generates.

--- -->

<!-- ## Views Customization

In order to override views delivered by Voyager DataTable, copy contents from ``vendor/joy/voyager-core/resources/views`` to the ``views/vendor/joy-voyager`` directory of your Laravel installation. -->

## Working Example

You can try laravel demo here [https://joy-voyager.kodmonk.com/api/documentation](https://joy-voyager.kodmonk.com/api/documentation).

## Documentation

Find yourself stuck using the package? Found a bug? Do you have general questions or suggestions for improving the joy voyager-core? Feel free to [create an issue on GitHub](https://github.com/rxcod9/joy-voyager-core/issues), we'll try to address it as soon as possible.

If you've found a bug regarding security please mail [gangwar.ramakant@gmail.com](mailto:gangwar.ramakant@gmail.com) instead of using the issue tracker.

## Testing

You can run the tests with:

```bash
vendor/bin/phpunit
```

## Upgrading

Please see [UPGRADING](UPGRADING.md) for details.

### Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email [gangwar.ramakant@gmail.com](mailto:gangwar.ramakant@gmail.com) instead of using the issue tracker.

## Credits

- [Ramakant Gangwar](https://github.com/rxcod9)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

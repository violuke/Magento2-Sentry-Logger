# Magento 2.1 Sentry Logger

This extension will add the ability to log to [Sentry](https://github.com/getsentry/). Default for the minimal logging level is DEBUG, this is set in the extensions di.xml.

Based on work by [Sebwite](https://github.com/Sebwite/Magento2-Sentry-Logger) but modified for my own use.

## Installation with composer (only option)
* Include the repository: `composer require violuke/magento2-sentry`
* Enable the extension: `php bin/magento --clear-static-content module:enable violuke_Sentry`
* Upgrade db scheme: `php bin/magento setup:upgrade`
* Clear cache

## Configuration
* Add the variable 'raven_dns' to your app/etc/env.php file. Example:

```
'raven_dns' => 'https://****@sentry.domain.com/8',
```

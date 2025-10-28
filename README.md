# SampleSyncApp [![Continuous Integration](https://github.com/aguilita1/SampleSyncApp2/actions/workflows/php.yml/badge.svg)](https://github.com/aguilita1/SampleSyncApp2/actions/workflows/php.yml) [![PHP Version](https://img.shields.io/badge/PHP-v8.4-blue)](https://www.php.net/ChangeLog-8.php) [![Alpine Linux Version](https://img.shields.io/badge/Alpine_Linux-v3.22-blue)](https://alpinelinux.org/releases/) [![Composer Version](https://img.shields.io/badge/Composer-v2.8-blue)](https://github.com/composer/composer/releases)
A reference implementation to demonstrate how to use Github Actions with a simple PHP CLI synchronization application.  A mirror of [SampleSnycApp](https://github.com/aguilita1/SampleSyncApp) that meant to test Renovate bot integration.
* Published Docker Images: [https://hub.docker.com/r/luigui/samplesyncapp2](https://hub.docker.com/r/luigui/samplesyncapp2)

## Docker Official Approved Base Images
* [PHP](https://github.com/docker-library/official-images/blob/master/library/php)
* [Composer](https://github.com/docker-library/official-images/blob/master/library/composer)

## Demonstrates Various Continuous Integration Tasks
* Checkout Code [``actions/checkout@v5``](https://github.com/marketplace/actions/checkout)
* Validate composer.json and composer.lock  ``run: composer validate --strict``
* Cache Dev Composer dependencies [``actions/cache@v4``](https://github.com/marketplace/actions/cache)
* Install DEV Dependencies [``php-actions/composer@v6``](https://github.com/marketplace/actions/composer-php-actions)
* PHP Static Analysis [``php-actions/phpstan@v3``](https://github.com/marketplace/actions/phpstan-php-actions)
* PHPUnit Tests [``php-actions/phpunit@v4``](https://github.com/marketplace/actions/phpunit-php-actions?version=v4)
* Install Prod Dependencies [``php-actions/composer@v6``](https://github.com/marketplace/actions/composer-php-actions)
* Setup Docker Buildx [``docker/setup-buildx-action@v3``](https://github.com/marketplace/actions/docker-setup-buildx)
* Docker Meta [``docker/metadata-action@v5``](https://github.com/marketplace/actions/docker-metadata-action)
* Login to Docker Hub [``docker/login-action@v3``](https://github.com/marketplace/actions/docker-login)
* Build and Push Docker Image [``docker/build-push-action@v6``](https://github.com/marketplace/actions/build-and-push-docker-images)
* Docker Scout [``docker/scout-action@v1``](https://github.com/marketplace/actions/docker-scout)
* Upload SARIF result [``github/codeql-action/upload-sarif@v4``](https://github.com/github/codeql-action)

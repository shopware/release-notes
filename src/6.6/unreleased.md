---
nav:
  title: v6.6.?.?
meta:
  date: "????-??-??"
---

# Release notes Shopware 6.6.?.?

## Abstract

This minor release contains some interesting features as well as technical improvements like Accessibility improvements and OpenTelemetry enhancements.

## System requirements

* tested on PHP 8.2 and 8.3
* tested on MySQL 8 and MariaDB 10.11

## Improvements

### Improve Redis configuration for platform

Redis is used in different places of Shopware, like cache, increments/locks/number ranges/messenger statistics.

To make it easier to configure and to have a better overview of the configuration, we improved the Redis configuration structure. There are few breaking changes, so please check the [changelog entry](https://github.com/shopware/shopware/blob/997d9c7fbf8848d623e4eff4aaa95d4fad16e130/changelog/_unreleased/2024-10-04-improved-redis-config-structure.md) for more information.

### Improve category and product indexing for many entities at once

To prevent exceeding the message size limit when indexing many entities at once, we improved the indexing process to split the entities into smaller chunks.

### Migrate admin-menu.store to pinia

The `adminMenu` store has been migrated from Vuex to Pinia. The store is now available as a Pinia store and can be accessed via `Shopware.Store.get(‘adminMenu’)`.

### Added support for opensearch sigv4 credential provider

We added the support for authentication with AWS OpenSearch using the SigV4 credential provider

### Added interface to support copy in batches

As a manufacturer of a flysystem adapter I want to be able to use the writeBatch-possibilities with a dedicated Interface until flysystem supports it out-of-the-box.

### Added vue to shopware object

## Fixed bugs

## Credits

Thanks to all diligent friends for helping us make Shopware better and better with each pull request!

## More resources

* [Detailed diff on Github](https://github.com/shopware/shopware/compare/v6.6.6.1...v6.6.7.0) to the former version
* [Changelog on GitHub](https://github.com/shopware/shopware/blob/v6.6.7.0/CHANGELOG.md) for this version.
* [Installation overview](https://developer.shopware.com/docs/guides/installation/)
* [Update from a previous installation](https://developer.shopware.com/docs/guides/installation/template.html#update-shopware)

## Get in touch

Discuss about decisions, bugs you might stumble upon, etc in our [community slack](https://shopwarecommunity.slack.com/). See you there ;)

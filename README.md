# Silverstripe Cloudflare boilerplate

Default modules for Silverstripe websites acting as an origin to a Cloudflare caching proxy.

<blockquote>
<p>By default, SilverStripe sends headers which signal to HTTP caches that the response should be not considered cacheable</p>
<cite><a href="https://docs.silverstripe.org/en/4/developer_guides/performance/http_cache_headers/">HTTP Cache Headers</a></cite>
</blockquote>

This boilerplate enables:
- HTTP cache header manipulation
- Page purge on publish/unpublish via the Cloudflare API
- Versioned record purging, if the record is represented by a URL

## Modules

+ [nswdpc/silverstripe-oldmantium](https://github.com/nswdpc/silverstripe-oldmantium) - reinforced Cloudflare support for versioned dataobjects
 + [cloudflare/sdk](https://github.com/cloudflare/cloudflare-php) - PHP SDK for Cloudflare
 + [symbiote/silverstripe-oldman](https://github.com/symbiote/silverstripe-oldman) - Simple cache purging for page records
+ [nswdpc/silverstripe-cache-headers](https://github.com/nswdpc/silverstripe-cache-headers) - modify HTTP cache headers sent by a Silverstripe website [more](https://github.com/nswdpc/silverstripe-cache-headers/blob/master/docs/en/001_index.md)

## Configuration

There is no configuration (yet) for this boilerplate. The defaults from included module configurations are used.

## Installation

The only supported way of installing this module is via [composer](https://getcomposer.org)

`composer require nswdpc/silverstripe-cloudflare-boilerplate`

## LICENSE

[BSD-3-Clause](./LICENSE.md)

## Maintainers

+ [dpcdigital@NSWDPC:~$](https://dpc.nsw.gov.au)

## Bugtracker

We welcome bug reports, pull requests and feature requests on the Github Issue tracker for this project.

Please review the [code of conduct](./code-of-conduct.md) prior to opening a new issue.

## Security

If you have found a security issue with this module, please email digital[@]dpc.nsw.gov.au in the first instance, detailing your findings.

## Development and contribution

If you would like to make contributions to the module please ensure you raise a pull request and discuss with the module maintainers.

Please review the [code of conduct](./code-of-conduct.md) prior to completing a pull request.

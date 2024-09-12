# Changelog
All notable changes to this project will be documented in this file.

## [0.29.0](https://github.com/omaxa-cen57039/openapi-typescript-codegen/compare/v0.28.0...v0.29.0) (2024-09-12)


### Features

* add andThen to CancelablePromise ([fd460dd](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/fd460dd12a1b6e2934d6a5895572e2a71bba8d7e))
* remove number suffix from operationId ([6e2e686](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/6e2e6867155f0984b84cc0542e3b6535b7724162))
* stuff ([5b88c62](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/5b88c62035b12567b72af1ab58cd684d33d73035))


### Bug Fixes

* adjust additional intermediate value call ([11f84f5](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/11f84f51ed4f045a0cf1cf1ad8b7287ecd79619a))
* adjust promise resolve for next issue ([41e25b8](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/41e25b86e22a70f342a1cf42f91f957d9c2b14f5))
* bump version ([605efa4](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/605efa4e53321d379a6304f5759611f8e43fe1f5))
* install release please ([7d1c869](https://github.com/omaxa-cen57039/openapi-typescript-codegen/commit/7d1c86989c7cb02711318c55edaabd73ec08a973))

## [0.27.0] - 2024-01-15
### Fixed
- Reverted `@apidevtools/json-schema-ref-parser` to version 10.1.0

## [0.26.0] - 2024-01-07
### Fixed
- Upgraded dependencies

## [0.25.0] - 2023-07-05
### Fixed
- Upgraded dependencies
### Added
- Allow usage of a custom axios instance
- Added message in generated files

## [0.24.0] - 2023-04-10
### Fixed
- Upgraded dependencies
- Fixed issue with Cancelable promise
- Fixed issue with escaping reserved keywords in schema names
### Added
- Added `--postfixModels` option

## [0.23.0] - 2022-06-02
### Fixed
- Upgraded dependencies
- Added blank line at the end of generated files
- Added support for Node.js v12
### Added
- Added `request` property inside `ApiError`
- Added support for `@depricated` inside models and operations

## [0.22.0] - 2022-04-26
### Fixed
- Upgraded dependencies
- Fixed issue with `null` value inside comments for OpenAPI v2 enums
- Fixed issue with compatibility for latest version of Axios (0.27.x)
### Removed
- Removed deprecated enum model generation

## [0.21.0] - 2022-04-06
### Fixed
- Return `undefined` to match `noImplicitReturns` rule
- Made `BaseHttpRequest` class abstract
- Removed private fields using `#` inside `CancelablePromise`
- Removed unneeded import `AbortController` from `node-fetch` client
- Filter out wrong enum values

## [0.20.1] - 2022-02-25
### Fixed
- Support enums with single quotes in names for V2

## [0.20.0] - 2022-02-25
### Fixed
- Updated dependencies
- Support enums with single quotes in names for V3
- Generating better names when `operationId` is not given (breaking change)
- Fixed issue where `x-enum` flags where breaking due to non-string values

## [0.19.0] - 2022-02-02
### Added
- Support for Angular client with `--name` option
- Added test cases for Angular client

## [0.18.2] - 2022-02-02
### Fixed
- Updated dependencies
- Fixed type definition
### Added
- Added test cases for CLI commands
- Added test cases for query parsing

## [0.18.1] - 2022-01-31
### Fixed
- Escaping error description
- Made `Client.request` and `BaseHttpRequest.config` props public

_## [0.18.0] - 2022-01-28
### Added
- Angular client generation!
- Updated documentation with more examples and better descriptions

## [0.17.0] - 2022-01-26
### Fixed
- Shorthand notation for properties passed through constructor
- Simplified creation of headers
- Prepare codebase for Angular client

## [0.16.2] - 2022-01-26
### Fixed
- Removed dependency on `URLSearchParams` to support browser and node without any additional imports

## [0.16.1] - 2022-01-26
### Fixed
- Correct export inside `index.ts` when giving a custom name

## [0.16.0] - 2022-01-25
### Added
- Added option to set the indentation (spaces and tabs)
- Added option to export separate client file that allows usage for multiple backends
### Fixed
- Decoupled OpenAPI object from requests
- Updated dependencies

## [0.15.0] - 2022-01-24
### Added
- Added change log and releases on GitHub

## [0.14.0] - 2022-01-24
### Fixed
- Added missing `postfix` options to typedef
- Updated escaping of comments and descriptions
- Better handling of services without tags
- Updated dependencies

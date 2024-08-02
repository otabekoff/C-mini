# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased] 🚀

### Added ✨
- **Added support for new currency conversion rates.**
- **Introduced a new module for advanced calculations.**
- **Add support for new API endpoints:** `/users` and `/orders` (#45) (Alice Meerkat)
- **Document `GET /orders` endpoint in the API documentation** (#48) (Bob Smith)

### Changed 🔄
- **Updated calculation algorithms for better accuracy.**
- **Refactored codebase to improve readability and performance.**
- **Breaking:** Modify response format for `GET /users` to include email field (#42) (Alice Meerkat)
- **Refactor `UserService` to improve performance** (#43) (Alice Meerkat, Carol Jones)

### Deprecated 🗑️
- **Deprecated the old conversion API.** The new API should be used instead.

### Removed ❌
- **Removed outdated functions from the utility module.**

### Fixed 🛠️
- **Fixed a bug that caused incorrect results in the currency conversion feature.**
- **Corrected minor typos in the documentation.**
- **Fix issue where `POST /orders` would fail with a 400 error for large payloads** (#47) (Bob Smith)
- **Correct typo in `GET /users` endpoint description** (#49) (Carol Jones)
- **Fix incorrect status code in `DELETE /users` response** (#41) (Bob Smith)
- **Fixed an issue with the date format in the report generation.**

### Security 🔒
- **Patched a vulnerability in the input validation mechanism.**

## [1.2.0] - 2024-08-02

### Added ✨
- **Add support for new API endpoints:** `/users` and `/orders` (#45) (Alice Meerkat)
- **Document `GET /orders` endpoint in the API documentation** (#48) (Bob Smith)

### Changed 🔄
- **Breaking:** Modify response format for `GET /users` to include email field (#42) (Alice Meerkat)
- **Refactor `UserService` to improve performance** (#43) (Alice Meerkat, Carol Jones)

### Fixed 🛠️
- **Fix issue where `POST /orders` would fail with a 400 error for large payloads** (#47) (Bob Smith)
- **Correct typo in `GET /users` endpoint description** (#49) (Carol Jones)

## [1.1.1] - 2024-07-15

### Fixed 🛠️
- **Fix incorrect status code in `DELETE /users` response** (#41) (Bob Smith)

## [1.1.0] - 2024-07-01

### Added ✨
- **Add `GET /users/{id}` endpoint for fetching user details** (#38) (Alice Meerkat)

### Changed 🔄
- **Update `GET /users` endpoint to support pagination** (#37) (Carol Jones)

## [1.0.0] - 2024-07-15

### Added ✨
- *Initial release with basic functionality including currency conversion and simple calculations.*

_See the [release notes](https://github.com/owner/name/releases/tag/v1.0.0) for details._

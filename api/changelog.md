# Changelog

All notable changes to v2 of the API will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

The versioning policy is based on the published [API Version Policy](https://localcontexts.org/support/api-guide/api-version-policy/).
For a changelog of all Hub updates, visit our [changelog](https://localcontexts.org/support/changelog/)
on our website.

<!--
    Major (X.0.0): MAJOR version increments indicate breaking changes
    Minor (0.X.0): MINOR version increments indicate non-breaking, additional functionality or
        new features with backward compatibility.
    Patch (0.0.X): PATCH version increments indicate non-breaking, bug fixes with backward
        compatibility.

    When adding a new version, update the version number in views.py > current_version variable
    based on the change type above.

    For badge customization, visit https://shields.io/badges.
    MAJOR BADGE: ![Static Badge](https://img.shields.io/badge/v2-MAJOR-orange?style=flat)
    MINOR BADGE: ![Static Badge](https://img.shields.io/badge/v2-MINOR-yellow?style=flat)
    PATCH BADGE: ![Static Badge](https://img.shields.io/badge/v2-PATCH-green?style=flat)
 -->
# Unreleased

## [2.3.0] - 2026-08-XX ![Static Badge](https://img.shields.io/badge/v2-MINOR-yellow?style=flat)
### Added
- GET Registry accounts call for integration partners at `/accounts` endpoint.

# Released
## [2.2.1] - 2026-03-19 ![Static Badge](https://img.shields.io/badge/v2-PATCH-green?style=flat)
### Fixed
- Fixed a bug where when going to the Open to Collaborate API call URL via a browser was throwing
a 500 error.

## [2.2.0] - 2025-10-15 ![Static Badge](https://img.shields.io/badge/v2-MINOR-yellow?style=flat)
### Added
- Added a variable in the API to allow users to increase the `page_size` of a page in the
Projects List. Default size is 10 projects per page, max size is 200 projects per page.

## [2.1.0] - 2025-10-01 ![Static Badge](https://img.shields.io/badge/v2-MINOR-yellow?style=flat)
### Added
- `external_ids` field added to Project and Multi-Project Detail calls match the new Project
external identifiers field.
- New `doi` search parameter added for future use.

### Changed
- Updated Project List API search for `publication_doi` and `providers_id` to include the updated
external IDs field. Search values for these two parameters will search through both the old and new fields.

## [2.0.3] - 2025-07-17 ![Static Badge](https://img.shields.io/badge/v2-PATCH-green?style=flat)
### Fixed
- Updated Project Details call in the API to remove previous Notice information for a Project
that now has Labels applied.

## [2.0.2] - 2025-05-16 ![Static Badge](https://img.shields.io/badge/v2-PATCH-green?style=flat)
### Changed
- Watermarked Notice and Label icons for sandbox API calls.

## [2.0.1] - 2025-04-13 ![Static Badge](https://img.shields.io/badge/v2-PATCH-green?style=flat)
### Changed
-API GET calls are now accessible even if the Hub is in maintenance mode.

## [2.0.0] - 2025-02-10 ![Static Badge](https://img.shields.io/badge/v2-MAJOR-orange?style=flat)
### Added
- v2 of the API
- OpenAPI documentation ([Swagger](https://localcontextshub.org/api/v2/docs/) and
[Redocly](https://localcontextshub.org/api/v2/redoc/))
- API key authentication
- Updated calls to include more fields (particularly in the Project Details call).

# TensionDev.ULID

# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [v1.1.0] - 2026-11-08
[v1.1.0](https://github.com/TensionDev/ULID/releases/tag/v1.1.0)

### Added
- Added ULID specification conformance tests for canonical encoding, case-insensitive parsing, overflow rejection, and Unix epoch timestamp handling.

### Changed
- Changed folder structure to match the TensionDev.ULID namespace.
- Changed target frameworks and added framework-specific optimizations.

### Fixed
- Fixed parsing to reject ULID strings whose first Base32 character exceeds `7`, preventing 130-bit overflow.
- Fixed timestamp construction to reject dates earlier than the Unix epoch instead of encoding a wrapped timestamp.


## [v1.0.0] - 2026-02-11
[v1.0.0](https://github.com/TensionDev/ULID/releases/tag/v1.0.0)

### Added
- Added TryParse for character spans.
- Added TryFormat for character spans.

### Fixed
- Fixed FromCrockfordBase32 to be case insensitive.
- Fixed FromCrockfordBase32 to accept 'o', 'O', 'i', 'I', 'l', 'L'.


## [v0.2.0] - 2025-05-01
[v0.2.0](https://github.com/TensionDev/ULID/releases/tag/v0.2.0)

### Added
- Added DateTime Conversion from ULID.

### Fixed
- Fixed Date Time implementation.
- Fixed ToString implementation.


## [v0.1.1] - 2025-02-02 [YANKED]
[v0.1.1](https://github.com/TensionDev/ULID/releases/tag/v0.1.1)

### Changed
- Changed Exception thrown message to a standardised string.


## [v0.1.0-alpha] - 2024-12-09
[v0.1.0-alpha](https://github.com/TensionDev/ULID/releases/tag/v0.1.0-alpha)

### Added
- Added ULID generated based on current system date and time.


# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

For each changelong entry sections are:

* `Added` for new features.
* `Changed` for changes in existing functionality.
* `Deprecated` for soon-to-be removed features.
* `Removed` for now removed features.
* `Fixed` for any bug fixes.
* `Security` in case of vulnerabilities.


## [Unreleased]

## [0.1.0] - 2020-06-12

This is the very first version of `enval`! This first version provides a way to validate the tools in your $PATH according to a `.enval.manifest.yaml` spec, so you can ensure you have the right versions to build and test your software project.

Thanks a lot to @hrodes, @figuerascarlos, @fllaca, @aagonzalezro, @aferrandini and @santiagoaldanondo for making it possible!

### Added

- Validation of tools in PATH according to version specs
- Support for following tools:
    - java
    - go
    - gotestsum
    - golangci-lint
    - node
    - npm
    - truffle
    - terraform
    - openapi-generator
    - swagger-cli
    - elixir
    - enval itself!
    - php
    - python
    - ruby
- Add `custom_specs` to add extra tools or override the default specs
- Support for tool flavors (for instance in **Java**: openjdk, oracle)

## [0.1.0-rc4] - 2020-05-27

### Fixed

- Fixed exit code when validation fails, changed from zero to one. 

## [0.1.0-rc3] - 2020-05-19

### Added

- Custom EnvalError implementation supporting error kinds [#45](https://github.com/Adhara-Tech/enval/issues/45)

### Fixed

- Memory access error when custom_specs folder doesn't exist [#49](https://github.com/Adhara-Tech/enval/issues/49)
- Stacktrace is shown when a spec wasn't found [#34](https://github.com/Adhara-Tech/enval/issues/34)

## [0.1.0-rc2] - 2020-05-10

### Added

- Document how to contribute to the project with new code or supported tools

### Fixed

- Implemented `custom_specs` [#38](https://github.com/Adhara-Tech/enval/pull/38), [#44](https://github.com/Adhara-Tech/enval/pull/44)

## [0.1.0-rc1] - 2020-05-08

First release candidate of `enval`

### Added

- Support for following tools:
    - java
    - go
    - gotestsum
    - golangci-lint
    - node
    - npm
    - truffle
    - terraform
    - openapi-generator
    - swagger-cli


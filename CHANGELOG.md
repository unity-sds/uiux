# Changelog

All notable changes for the Unity UI/UX Service Team will be documented in this file. This combines changes across multiple repositories.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

--------

## [Unity Release 24.1] - 2024-04-15

### Repository Tags

- [unity-py](https://github.com/unity-sds/unity-py) : [0.4.0](https://github.com/unity-sds/unity-py/releases/tag/0.4.0)
- [unity-ui](https://github.com/unity-sds/unity-ui) : [0.5.0](https://github.com/unity-sds/unity-ui/releases/tag/0.5.0)
- [unity-ui-infra](https://github.com/unity-sds/unity-ui-infra) : [0.1.0](https://github.com/unity-sds/unity-ui-infra/releases/tag/0.1.0)
- [sounder-sips-tutorial](https://github.com/unity-sds/sounder-sips-tutorial) : [1.0.0](https://github.com/unity-sds/sounder-sips-tutorial/releases/tag/1.0.0)

### Added

#### unity-ui
* Updated Navbar CSS styling to match Figma designs [#5](https://github.com/unity-sds/unity-ui/issues/5)
* Added CI/CD workflow to build application as a docker image. [#21](https://github.com/unity-sds/unity-ui/issues/21)
* Updated application build configuration. Stateful information has been removed from project configuration. Instead we now allow environment variables to be supplied to the container at startup which in turn get injected into the Unity UI Codebase. This is in support of moving to dynamic configuration of the application via Unity Marketplace. Related to [#3](https://github.com/unity-sds/unity-sds-portal/issues/3)

#### unity-py
* We've added the ability to override settings in the default config file by passing in a config file with the settings needing to be overridden when instantiating a Unity object. 56
* Collection creation (create_collection) through dataService library
* Added support for defining custom metadata for project and venue.
* Added methods to return STAC content instead of unity domain objects if requested
* Added properties parsing of stac metadata to dataset objects

#### unity-ui-infra
* Initial attempt at updating information in README after creating repo. by @anilnatha in [#2](https://github.com/unity-sds/unity-ui-infra/issues/2)
* Added initial terraform configuration files to support marketplace by @anilnatha in [#3](https://github.com/unity-sds/unity-ui-infra/issues/3)

#### sounder-sips-tutorial
* Updates to utilize unity-py client, custom metadata, collection creation notebooks, data access notebooks, and more.

### Fixed

### Changed

#### unity-py

* Updated get_collections and get_collection_data to support limit parameter.
* Updated get_collection_data to support filter parameter which takes CQL string.

### Removed

### Security

### Deprecated



## [Unity Release 23.1] - 2023-04-17

### Repository Tags

- [unity-py](https://github.com/unity-sds/unity-py) : [0.1.0](https://github.com/unity-sds/unity-py/releases/tag/0.1.0)
- [sounder-sips-tutorial](https://github.com/unity-sds/sounder-sips-tutorial) : [0.1.0](https://github.com/unity-sds/sounder-sips-tutorial/releases/tag/0.1.0)

### Added

#### Unity-Py Updates

* Added Services and Classes to ecapsulate funcionality per Unity Service Area
    1. Process Service & Class — Deploy a process, List processes, get metadata about a processes, query jobs per process, execute a job
    2. Job Class — Facilitate API calls to U-SPS to monitor jobs, get job results, or dismiss jobs.
    3. Application Service — Courtesy of James and Masha (See Application Registry below).
* Mercury Dashboard Example
* Miscellaneous quality of life improvements to ease code developing (type hinting, annotations, etc)

#### Tutorial Notebook Updates

* Application Service Tutorial Notebook — Courtesy of James and Masha (See Application Registry below).
* Cleanup of Sounder SIPS Tutorial Jobs Notebook — Updated instructions and terminology, showcasing how to deploy a process using a JSON payload (was removed previously).

#### Application Registry
* [unity-ads-deployment #79](https://github.com/unity-sds/unity-ads-deployment/issues/79) Add Dockstore API access to Unity.py
* [unity-ads-deployment #87](https://github.com/unity-sds/unity-ads-deployment/issues/87) Convert Unity.py Application Package API to use Hosted Workflows


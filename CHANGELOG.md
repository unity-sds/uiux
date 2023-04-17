# Changelog

All notable changes for the Unity UI/UX Service Team will be documented in this file. This combines changes across multiple repositories.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

--------

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


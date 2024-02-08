# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Known Issues]
- None. Please feel free to submit an issue via [GitHub](https://github.com/ryanblenis/MeshCentral-ScriptTask) if you find anything.

## [0.0.19] - 2024-02-07
### Fixed
- Merge PR fixing scroll bars and Powershell execution policy

## [0.0.18] - 2022-03-12
### Fixed
- Compatibility with MeshCentral => 0.9.98 (promise requirement removed from MeshCentral, nedb moved to @yetzt/nedb)

## [0.0.17] - 2021-10-07
### Fixed
- Compatibility with MeshCentral > 0.9.7

## [0.0.16] - 2021-05-18
### Fixed
- Drag/drop scripts between folders

## [0.0.15] - 2020-03-07
### Fixed
- Prevent race condition with conflicting plugins changing the app views directory by using absolute paths

## [0.0.14] - 2020-02-28
### Added
- Add new script from ScriptTask plugin without dragging/uploading an existing script
- Variables introduced. Supports global, script, mesh, and node level. Overridden in that order.

## [0.0.13] - 2020-02-15
### Fixed
- Folder rename function now working as intended
- Removed ability to "edit" folders as if they were a script

## [0.0.12] - 2020-02-14
### Fixed
- Rename function broke when filetype tags were added

## [0.0.11] - 2020-01-24
### Added
- Advanced selection of nodes based on mesh and tag membership

## [0.0.10] - 2020-01-02
### Fixed
- Removed logging to MeshCentral events DB for each script run / refresh event (causing events file to grow quickly and crash NeDB instances)

## [0.0.9] - 2019-12-24
### Fixed
- Native Powershell scripts now run correctly on more versions of Linux/MacOS

## [0.0.8] - 2019-12-23
### Fixed
- Force strip carriage returns from bash scripts

## [0.0.7] - 2019-12-23
### Fixed
- Some versions of Linux don't default the agents root to the MeshAgent's directory. Added path detection for a safe temp zone. Thanks /u/Reverent for the assist in debugging that one!

## [0.0.6] - 2019-12-23
### Added
- Status return of a script as success/failure if the script does not produce output
- Endpoint debugging toggle via console (plugin scripttask debug)
### Fixed
- Made some endpoint calls a little safer with try/catch to stop errors from killing the process

## [0.0.5] - 2019-12-22
### Added
- NeDB support
### Fixed
- CSS call looking for mapping file removed
- Date/time select on schedule screen might not have had the correct mimetype, thus not appeared in some instances

## [0.0.4] - 2019-12-22
### Added
- Script type identifier to the script tree view
### Fixed
- Prevent catch-up jobs from running every minute on long running schedules when a node is offline for a period of time.
- Check for scheduled jobs 1 minute in the future to prevent schedules running 1 minute behind intended time.

## [0.0.3] - 2019-12-20
### Fixed
- Typo causing installs to think Mongo is not in use

## [0.0.2] - 2019-12-20
### Added
- Suppressed errors and made a nice error message for those without MongoDB (currently unsupported)

## [0.0.1] - 2019-12-20
### Added
- Released initial version

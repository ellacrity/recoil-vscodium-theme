# Change Log

All notable changes to the "recoil" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [0.5.0] - 2023-08-14

### Added
- New colors added to palette, such as Bone White, Tan and variants of existing colors
- Better/increased support for `Go` and `Zig` (and basic Python)
  - Over time, expect better support for these languages (particularly for Go and Zig)

### Changed
- Naming scheme for textmate rules slightly changed (WIP)
  - Names all use `(Unset)` suffix if they remove `fontStyle` property; else `(Normal)` if they allow `fontStyle` passthrough

## [0.4.6] - 2023-07-19

### Changed

- Decoupled deployment workflows into two separate jobs
  - One of the jobs failing caused the entire workflow to fail

## [0.4.5] - 2023-07-19

### Fixed

- Bumped extension version to force update on Open VSX registry

## [0.4.4] - 2023-07-18

### Changed

- Updated the display name of the extension to simply "Recoil"
  - The previous name "Recoil - Theme" was deemed redundant

## [0.4.3] - 2023-07-18

### Added

- `.nvmrc` file to declare the Node.js version used

### Changed

- Updated `cd.yml` workflow to match push and pull requests to `main`
- Started replacing "semanticTokenColorCustomizations" overrides with textMate rules
- Improved support for TOML files
- Changed UI foreground colors for some components to a yellow-tinted "white"

### Removed

- Unused rules and (some) duplicate entries

## [0.4.2] - 2023=07-17

### Changed

- Modified deployment workflow to include both VSCode and VSCodium

## [0.4.1] - 2023-07-17

## Changed

- Bumped the version to `0.4.1` as workaround for publishing the same version

## [0.4.0] - 2023-07-17

### Added

- Add preliminary support for Go
- Begin actve keeping of change log for end-users to keep track of project changes

### Changed

- Foreground and background colors in explorer made more legible
- Git foreground colors modified for more consistent UI
- Increase contrast for list item state and various UI components

## [0.3.7] - 2023-07-03

### Changed

- GitHub Actions now automatically deploys to Open VSX

## [0.3.2] - 2023-07-03

### Changed

- GitHub Actions now automatically deploys to Open VSX

## [0.0.1] - 2023-03-24

- Initial release
  - **Warning**: this project is not yet stable. Please refer to the [README](/README.md).
- Generic support provided for Rust projects and related file types
  - Rust source code
  - TOML
  - YAML
  - JSON

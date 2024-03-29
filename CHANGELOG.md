# Change Log

All notable changes to the "recoil" extension will be documented in this file.

## [0.8.0] - Unreleased

This represents the set of pending changes that have not yet been implemented, or are still in the works.
As this project is not my main focus and exists solely so that I have somewhere to store my theme, it is
not a top priority. With that said, I will try my best to keep it as up-to-date as possible.

### Added

- Automation tooling to remove duplicate entries and accidental overriding
  - The theme file is read from top to bottom, with rules at the bottom overriding whatever has been set above
- MVP algorithm for parsing, sorting and validating the color scheme

### Changed

- Theme is now modified with a CLI tool to make it easier to insert new entries, make modifications, and more without having to worry about breaking the color palette.

## [0.7.4] - 2023-12-04

### Added

- Improved support for Python, JavaScript and TypeScript/TSX. There should be fewer uncolored tokens now.
  - If you find uncolored tokens, please open an issue if you would like them to be fixed

### Changed

- Modified variable and parameter tokens to be tan rather than blue hue to be more consistent with the rest of the theme.
- **Slight tweaks** were made to the overall color palette, which should result in tokens standing out a bit more, improving legibility.

### Fixed

- Invalid / illegal tokens should now be fixed. They were appearing as bold, bright white, which was quite jarring to look at. Instead, they are now the default foreground color but the red squiggle remains.

## [0.7.3] - 2023-11-28

This release comprises a set of changes that have been pending for quite a while. I have not had the
time to sit down and merge these changes with the theme. The theme will now reflect these changes in
the Open VSIX store for VSCodium and the extension marketplace for VSCode.

### Added

- Add preliminary support for C and C++
- Added additional surface colors to make tabs and other elements stand out easier (UI/improvements)

### Changed

- Existing theme colors may have been modified slightly since the past release in order to make room
  for additional languages without risking excessive color clashing.

## [0.7.2] - 2023-09-27

### Added

- More semantic tokens and colors are available for Zig
- Added color palette/theme variants

## [0.7.1] - 2023-09-22

### Added

- Added a new section to the README document to tell users how to override colors.

### Fixed

- Colors are now more consistent across languages with keyword specialization that should cover most cases.

### Removed

- Removed the theme variant "Vivid" (for now). I would like to add more themes, but I cannot due to time constraints.

## [0.7.0] - 2023-09-22

### Added

- Added the new theme variant "Vivid"

## [0.6.15] - 2023-09-21

This release is cummulative; mostly backlog that is being finally published.

### Added

- More Zig code is supported via semantic tokens and TextMate rules

### Changed

- Modified control flow keywords in Rust to make them stand out more
- Changed Zig's palette to more accurately reflect semantic meaning
  - **NOTE**: I just started learning Zig, so please bear with me as I continue to experiment and then push changes to `main` + publish. I typically make small changes as I go, saving to my local settings. After a while, I batch update this theme. If you want to help, you are more than welcome to!
- Changed some colors regarding control flow in Zig

## [0.6.8] - 2023-09-15

### Fixed

- Fixed accidental insertion of global "function" override
  - This may or may not result in other languages losing color for function types.
  - This will be addressed if that is the case.

## [0.6.7] - 2023-09-15

### Fixed

- Removing "keyword.other.rust" TextMate rule caused no colors for certain keywords.
  - This is temporarily being added back in until a better solution is found

## [0.6.6] - 2023-09-15

### Added

- Added better color support for JavaScript / TypeScript (still rudimentary)
- Support for Zig is officially added
  - ZLS unfortunately does not emit as much semantic token information as is needed to create a complete theme but as improvements are made, this project will be updated.

### Changed

- Operator specialization now means that colors are more consistent and puncutation was made easier to differentiate, etc.
- Theme palette and general color scheme was iteratively improved

### Removed

- Duplicate entries where found
  - This process is still not yet automated. Soon, it will be via a simple JSON parser to insert/remove color rules

## [0.6.0] - 2023-08-21

### Changed

- Theme has been overhauled to conform to new color palette

## [0.5.2] - 2023-08-20

### Added

- Better support for Rust declarative macros (`macro_rules!` items)
- Continued incremental support for the Zig programming language

### Changed

- Primary foreground color now uses an amber hue rather than blue for better contrast
- Overview ruler colors were changed to be more consistent with VCS (Git) colors
- Operators are now bright blue by default to improve visibility

### Fixed

- GitHub Actions workflows now use the latest LTS version of Node.js

## [0.5.1] - 2023-08-17

### Added

- Expanded semantic token support for Zig
- Editor bracket and indent / scope guide colors to match current palette

### Changed

- Removed color overrides in favor of more precise TextMate rules

### Fixed

- Several instances of "semanticTokenColors" were incorrectly overriding colors
  - Most overrides exist on purpose; many still do not and may not be necessary

### Removed

- Extraneous comments and leftover artifacts from the theme file were deleted

## [0.5.0] - 2023-08-14

### Added

- New colors added to palette, such as Bone White, Tan and variants of existing colors
- Better/increased support for `Go` and `Zig` (and basic Python)
  - Over time, expect better support for these languages (particularly for Go and Zig)

### Changed

- Naming scheme for TextMate rules slightly changed (WIP)
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
- Started replacing "semanticTokenColorCustomizations" overrides with TextMate rules
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

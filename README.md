# Recoil

[`recoil`][project-repo] is a dark theme for VSCodium with a focus on providing full semantic token support for various programming languages.

## Language Support

Currently, the primary target is Rust. However, this theme also supports the following languages and markup langauges:
- [`Rust`][rust]: crates and workspaces
- [`TOML`][toml]: schema files related to Rust development (Cargo, Rustfmt)
- [`JSON`][json]: json/jsonc configuration and settings files
- [`YAML`][yaml]: yaml/yml schema files
- "Best-effort" support for a variety of random languages and formats

### Future Goals

Support will be added for more languages over time. There is currently only a single contributor, so if you would like to see something added, please consider [contributing to the project](#contributing).

Language support is in the works for [`Go`][golang], and [`Zig`][zig] will likely follow soon after that.

## Installation

This extension can be found on [Open VSX][open-vsx]. This option is the easiest and most straightforward. [Install the extension](#open-vsx), enable it and you should be all set. From there, you may customize the theme as you see fit.

To build the project from source, please see: [Building from Source](#building-from-source).

### Open VSX

[Open VSX][open-vsx] allows you to install `recoil` just as you would any other extension.

After installation is complete, simply set your color theme to `Recoil`.

### Building from Source

This is free software. As such, the source code is hosted publicly and made available to anyone that wishes to view the source code.

The extension is currently [hosted on GitHub][project-repo]. You can clone it, modify it, fork it or do whatever you like with it.

To build this project manually, from source:

- Clone the repository
- `cd` into the repository
- Run the `build` script using `npm run build`
- Install the VSIX (VSCodium extension)
   - From your terminal console (see below).
   - Right-click on the generated __vsix__ file, then __`Install Extension VSIX`__
   - Run the following command within VSCodium: __`Extensions: Install from VSIX`__
   
```shell
git clone https://github.com/ellacrity/recoil-vscodium-theme
cd recoil-vscodium-theme
npm run build
# Substitute ${version} with the version number defined in the `package.json` file.
codium --install-extension recoil-${version}.vsix
```

## Stability

I will do my best to follow semantic versioning, but there may be occasions where an accidental breaking change occurs. If this happens, please open an issue and I will get to it as quickly as possible.

## Contributing

Open a new ticket that outlines the scope of your contribution(s) and be ready to discuss your changes.

If your changes are approved, open a pull request and I will review your changes. If everything looks good, I will merge your contribution.

Following the above steps is the best way to ensure your contribution is accepted.

## License

This project is licensed under the [MIT license][license].

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in
[`recoil`][project-repo] by you, shall be licensed as MIT, without any additional terms or conditions.

<!-- Links section -->

[project-repo]: https://github.com/ellacrity/recoil-vscodium-theme
[license]: https://github.com/ellacrity/recoil-vscodium-theme/blob/main/LICENSE
[nerd-fonts]: https://github.com/ryanoasis/nerd-fonts
[open-vsx]: https://open-vsx.org/

<!-- Languages -->
[rust]: https://www.rust-lang.org/
[json]: https://www.json.org/
[toml]: https://toml.io/en/
[yaml]: https://yaml.org/
[golang]: https://go.dev/
[zig]: https://ziglang.org/

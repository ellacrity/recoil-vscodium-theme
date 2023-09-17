# Recoil

[`Recoil`][project-repo] is a colorful dark theme centered around my daily workflow as a systems programmer.

## Description

This extension provides the kind of color theme that I simply could not find anywhere, despite looking for
hours. Every theme had defects, or missing features that I needed for maximum productivity. Instead of putting
together a "solution" which simply overrided some common theme, I created my own from the ground up.

### Should I use This?

This theme is tailored to my specific needs, and I make incremental changes using an iterative approach to
development. I do work extensively with [`Rust`][rust-lang], but occasionally with [`Go`][go-lang] for network-based
tools. More recently, I have discovered a wonderful language called "[`Zig`][zig-lang]". Basic, functional support
exists for `Zig` and it will likely be prioritized when applying updates to this theme.

**TL;DR**: If you do not work with the languages listed above, then this extension is probably not for you! And that is okay! Also, if you would like to see a language added and don't mind helping out, I would absolutely love contributions!!

## Development Status

This project is currently under **active development**.

### Registries

This extension is available for both VSCodium
vailable for both VSCodium and VSCode.

The goal for this project is to provide custom themes based on a shared palette. Variants will be introduced to the project in the near future.

for VSCodium with a focus on providing full semantic token support for various programming languages.

### Official Language Support

The following languages and serialization formats are supported:

- [`Rust`][rust-lang]: crates and workspaces
- [`Zig`][zig-lang]: crates and workspaces
- [`Go`][go-lang]: crates and workspaces
- [`TOML`][toml-fmt]: schema files related to Rust development (Cargo, Rustfmt)
- [`JSON`][json-fmt]: json/jsonc configuration and settings files
- [`YAML`][yaml-fmt]: yaml/yml schema files

If you find that something is missing, or inconsistent, please feel free to open an issue so we can address it as quickly as possible. Thanks!

## Future Goals

- [ ] Continued, iterative development for existing languages
- [ ] Addition of more languages
- [ ] Automate generation of the color scheme
  - [ ] Automate a parser that reads an input theme file
  - [ ] Alphabetize the input file and remove duplicate entries
  - [ ] Expand CI/CD automation capabilties with scripts and/or binaries
- [ ] Automatic validation of color scheme
  - [ ] Rules that violate the schema will be removed automatically
  - [ ] Add interactive mode to avoid accidental removal of needed entries

### Contributors Needed

Incremental support for more and more languages will be added over time. There is currently only a single contributor (myself), and I have a have many things going on right now, so I could really use help maintaining this extension.

If you would like to see something added, please consider [contributing to the project](#contributing).

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
  - Right-click on the generated **vsix** file, then **`Install Extension VSIX`**
  - Run the following command within VSCodium: **`Extensions: Install from VSIX`**

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

<!-- Local Links -->

[license]: https://github.com/ellacrity/recoil-vscodium-theme/blob/main/LICENSE
[changelog]: /CHANGELOG.md
[themes]: /themes

<!-- Links section -->

[project-repo]: https://github.com/ellacrity/recoil-vscodium-theme
[nerd-fonts]: https://github.com/ryanoasis/nerd-fonts
[open-vsx]: https://open-vsx.org/

<!-- Programming Languages -->

[go-lang]: https://go.dev/
[rust-lang]: https://www.rust-lang.org/
[zig-lang]: https://ziglang.org/

<!-- Serialization Formats -->

[json-fmt]: https://www.json.org/
[toml-fmt]: https://toml.io/en/
[yaml-fmt]: https://yaml.org/

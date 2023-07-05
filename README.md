# Recoil

[`recoil`][project-repo] is a dark theme for VSCodium. It is meant for my own
personal use.

## Disclaimer

This project is for my own personal use. Support for particular programming languages is not
guaranteed, but I will accept pull requests and modifications to improve it.

## Installation

Unfortunately, Microsoft does not provide first-class support for VSCodium extensions. As such,
you may need to build and install it from source. I recently published this extension to the
[`Open VSX Registry`][open-vsx], so you should be able to install it just like any other extension.

### Building from Source

The source code to this project is freely available on GitHub, so it can be built from source very
easily.

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
# Depending on the version of the extension, the following command may need to be modified:
codium --install-extension recoil-0.3.5.vsix
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

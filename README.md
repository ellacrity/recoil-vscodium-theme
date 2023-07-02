# Recoil

[`recoil`][project-repo] is a customized theme that I use when using VSCodium.

I do not guarantee support, as this for my personal use. 

## Installation

Currently, since Microsoft does not really provide any kind of true support for VSIX extensions that **are not** specifically for VSCode, this extension must be manually installed.

### Installing from OpenVSIX

### Building from Source

To build this project from source:
1. Clone the repository
2. `cd` into the repository
3. Run the `build` script using `npm run build`
4. Install the VSIX (VSCodium extension)
   1. From your terminal console (see below).
   2. Right-click on the generated __vsix__ file, then __`Install Extension VSIX`__
   3. Run the following command within VSCodium: __`Extensions: Install from VSIX`__
   
```shell
git clone https://github.com/ellacrity/recoil-vscodium-theme
cd recoil-vscodium-theme
npm run build
# Depending on the version of the extension, the following command may need to be modified:
codium --install-extension recoil-0.3.5.vsix
```

## Customizations

### Fonts

Here is an example taken from my 'settings.json` file showing font family settings:
```jsonc
{
  "editor.codeLensFontFamily": "'VictorMono Nerd Font', monospace",
  "editor.fontFamily": "'VictorMono Nerd Font', monospace",
  "editor.inlayHints.fontFamily": "'VictorMono Nerd Font', monospace",
  "errorLens.fontFamily": "'VictorMono Nerd Font', monospace",
  "markdown.preview.fontFamily": "Quicksand, Inter, system-ui, sans-serif",
  "terminal.integrated.fontFamily": "'VictorMono Nerd Font', monospace",
  /* VictorMono is a thin font, so using 500 (medium) as default improves legibility */
  "editor.fontWeight": "500",
}
```

### Installing Custom Fonts

These fonts can usually be installed using your built-in package manager ([`apt`][apt]/[`apt-get`][apt], [`pacman`][pacman], [`pamac`][pamac], [`yum`][yum], etc.).

If you use Arch Linux, you cna easily install [`VictorMono Nerd Font`][victor-mono-nerd] with :
```shell
sudo pacman -S ttf-victor-mono-nerd
```


* NOTE: Depending on your operating system, the way you installed it, and other unknown factors, the naming convention outlined above may not work.
  * If your system is not detecting the font, try using 'VictorMono NF' instead of 'VictorMono Nerd Font' and vice versa.
  
*  font may be referred to as "VictorMono Nerd Font" or "VictorMono NF", . You will need to try both to see which works. If neither works, then it is probably not installed on your system.

## Hacking

## Extending the Theme

If you use rainbow brackets, you will need to set them in your own personal `settings.json` file.

For your reference, my settings are as follows:
```jsonc
{
  "workbench.colorCustomizations": {
    "editorBracketHighlight.foreground1": "#ABB3BA",
    "editorBracketHighlight.foreground2": "#F7A76E",
    "editorBracketHighlight.foreground3": "#90F76E",
    "editorBracketHighlight.foreground4": "#ABB3BA",
    "editorBracketHighlight.foreground5": "#6EECF7",
    "editorBracketHighlight.foreground6": "#A76EF7",
    "editorBracketPairGuide.activeBackground1": "#ABB3BA80",
    "editorBracketPairGuide.activeBackground2": "#F7A76E80",
    "editorBracketPairGuide.activeBackground3": "#90F76E80",
    "editorBracketPairGuide.activeBackground4": "#ABB3BA80",
    "editorBracketPairGuide.activeBackground5": "#6EECF780",
    "editorBracketPairGuide.activeBackground6": "#A76EF780",
    "editorBracketPairGuide.background1": "#ABB3BA40",
    "editorBracketPairGuide.background2": "#F7A76E40",
    "editorBracketPairGuide.background3": "#90F76E40",
    "editorBracketPairGuide.background4": "#ABB3BA40",
    "editorBracketPairGuide.background5": "#6EECF740",
    "editorBracketPairGuide.background6": "#A76EF740"
  }
}
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
[`recoi`][project-repo] by you, shall be licensed as MIT, without any additional terms or conditions.

<!-- Links section -->

[project-repo]: https://github.com/ellacrity/recoil-vscodium-theme
[license]: https://github.com/ellacrity/recoil-vscodium-theme/blob/main/LICENSE
[victor-mono-nerd]: https://github.com/ryanoasis/nerd-fonts

<!-- Package managers-->
[apt]: https://en.wikipedia.org/wiki/APT_(software)
[pacman]: https://wiki.archlinux.org/title/pacman
[pamac]: https://wiki.manjaro.org/index.php/Pamac
[yum]: https://www.redhat.com/sysadmin/how-manage-packages

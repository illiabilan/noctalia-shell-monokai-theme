# Monokai Pro Theme for Noctalia Shell

An unofficial port of the [Monokai Pro](https://monokai.pro) theme for [noctalia-shell](https://github.com/noctalia-dev/noctalia-shell), a Hyprland shell.

<p align="center">
  <img src="https://assets.noctalia.dev/noctalia-logo.svg?v=2" alt="Noctalia Logo" style="width: 192px" />
</p>

<p align="center">
  <a href="https://docs.noctalia.dev/getting-started/installation">
    <img
      src="https://img.shields.io/badge/🌙_Install_Noctalia-A8AEFF?style=for-the-badge&labelColor=0C0D11"
      alt="Install Noctalia"
      style="height: 50px"
    />
  </a>
</p>

<p align="center">
  <a href="https://github.com/noctalia-dev/noctalia-shell/commits">
    <img src="https://img.shields.io/github/last-commit/illiabilan/noctalia-shell-monokai-theme?style=for-the-badge&labelColor=0C0D11&color=A8AEFF&logo=git&logoColor=FFFFFF&label=commit" alt="Last commit" />
  </a>
  <a href="https://github.com/noctalia-dev/noctalia-shell/stargazers">
    <img src="https://img.shields.io/github/stars/illiabilan/noctalia-shell-monokai-theme?style=for-the-badge&labelColor=0C0D11&color=A8AEFF&logo=github&logoColor=FFFFFF" alt="GitHub stars" />
  </a>
  <a href="https://docs.noctalia.dev">
    <img src="https://img.shields.io/badge/docs-A8AEFF?style=for-the-badge&logo=gitbook&logoColor=FFFFFF&labelColor=0C0D11" alt="Documentation" />
  </a>
  <a href="https://discord.noctalia.dev">
    <img src="https://img.shields.io/badge/discord-A8AEFF?style=for-the-badge&labelColor=0C0D11&logo=discord&logoColor=FFFFFF" alt="Discord" />
  </a>
</p>

## Project Structure

```
MonokaiPro/
├── MonokaiPro.json          # Shell color scheme (Dark & Light modes)
└── terminal/
    └── kitty/
        ├── MonokaiPro-dark.conf   # Kitty dark theme
        └── MonokaiPro-light.conf  # Kitty light theme
```
## Features

- **Dark Mode**: Fully supported theme for both the shell and Kitty terminal
- **Light Mode**: Available but not fully adopted yet
- **Kitty Terminal Support**: Includes color schemes for Kitty terminal emulator

## Installation

To install and use this theme:

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/monokai-pro-noctalia.git
   cd monokai-pro-noctalia
   ```

2. Copy the `MonokaiPro` folder into your noctalia configuration directory:
   ```bash
   cp -r MonokaiPro ~/.config/noctalia/colorscheme/MonokaiPro/
   ```

3. (Optional) Clean up by removing the cloned repository folder:
   ```bash
   cd ..
   rm -rf monokai-pro-noctalia
   ```

2. To apply the theme, relogin or restart your noctalia shell. The theme will then appear in your shell settings.

## Usage

### Shell Theme

The `MonokaiPro.json` file contains color definitions for both dark and light modes that noctalia-shell uses to theme the interface.

### Kitty Terminal

You can apply the Kitty terminal theme either automatically or manually:

- **Automatic:** In noctalia shell settings, enable the Kitty template for color schemes. The Kitty theme will then be applied automatically whenever you change the shell theme.
- **Manual:** Add the following to your `~/.config/kitty/kitty.conf` to include the dark theme:
  ```conf
  include ~/.config/noctalia/colorscheme/MonokaiPro/terminal/kitty/MonokaiPro-dark.conf
  ```
  Or, for the light theme:
  ```conf
  include ~/.config/noctalia/colorscheme/MonokaiPro/terminal/kitty/MonokaiPro-light.conf
  ```
  Alternatively, copy the desired `.conf` file to your Kitty config directory and include it as needed.

## Note

⚠️ **Light mode is not fully adopted yet** - While the light mode theme files are included, they may not be fully compatible with all noctalia-shell components.

## License

See [LICENSE](LICENSE) file for details.

## Credits

Based on the [Monokai Pro](https://www.monokai.pro/) color scheme.

# project-epoch on Linux 

## Requirements

The `download-patches` script requires `aria2` to function. Install `aria2` using your distribution's package manager:

- **Debian / Ubuntu / Bazzite**:
    ```sh
    sudo apt update
    sudo apt install aria2
    ```
- **Arch / Manjaro**:
    ```sh
    sudo pacman -S aria2
    ```
- **Fedora**:
    ```sh
    sudo dnf install aria2
    ```

## Wine Prefixes and Bottles

A *Wine prefix* is a directory that contains a separate Wine environment, including its own registry, configuration, and installed programs. This allows you to isolate different Windows applications.

- **Bottles** is a graphical tool for managing Wine prefixes. It simplifies creating, configuring, and running different Wine environments.
- **Wine** itself can be used directly to create and manage prefixes using the `WINEPREFIX` environment variable.

For example, to create a new Wine prefix:
```sh
WINEPREFIX=~/mywineprefix winecfg
```

To use Bottles, install it from your distribution's package manager or Flatpak, then follow the GUI to create and manage prefixes.


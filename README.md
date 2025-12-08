# affinity-everywhere

This is a sister project to https://github.com/mrshmllow/affinity-nix,
which allows you to run the Affinity suite of applications on any Linux distro through AppImages.

**You can download the latest AppImage [here](https://github.com/mrshmllow/affinity-everywhere/releases/latest).**

## Preamble

The prefix is located in `$XDG_DATA_HOME/affinity/` or `$XDG_DATA_HOME/affinity-v3/` falling back to `$HOME/.local/share/affinity/` or `$HOME/.local/share/affinity-v3/`.

## Usage

Double click them!

### CLI Usage

Additionally, each AppImage (`v3|photo|designer|publisher`) has the following extra functionality:

```sh
$ affinity-v3.AppImage --help
Usage: affinity-v3 [COMMAND] [OPTIONS]

Commands:
  wine
  winetricks
  wineboot
  wineserver
  update|repair|install   Update or repair the application
  help                    Show this
  (nothing)               Launch Affinity v3

```

> [!TIP]
> Armed with these you should be able to follow https://affinity.liz.pet/v2/misc-troubleshooting/ for troubleshooting steps.

For example, accessing `wine`:

```sh
$ affinity-v3.AppImage wine
Usage: wine PROGRAM [ARGUMENTS...]   Run the specified program
       wine --help                   Display this help and exit
       wine --version                Output version information and exit

```

Or `winecfg`:

```sh
$ affinity-v3 wine winecfg
```


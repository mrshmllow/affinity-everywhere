# affinity-everywhere

This is a sister project to https://github.com/mrshmllow/affinity-nix,
which allows you to run the Affinity suite of applications on any Linux distro through AppImages.

**You can download the latest AppImage [here](https://github.com/mrshmllow/affinity-everywhere/releases/latest).**

## Preamble

The prefix is located in `$XDG_DATA_HOME/affinity/` falling back to `$HOME/.local/share/affinity/`.

## Usage

Double click them!

### CLI Usage

Additionally, each AppImage (`photo|designer|publisher`) has the following extra functionality:

```sh
$ ./affinity-photo-2.6.4.AppImage --help
Usage: affinity-photo-2 [COMMAND] [OPTIONS]

Commands:
  wine
  winetricks
  wineboot
  wineserver
  update|repair|install   Update or repair the application
  help                    Show this
  (nothing)               Launch Affinity Photo 2

```

> [!TIP]
> Armed with these you should be able to follow https://affinity.liz.pet/docs/misc-troubleshooting.html for troubleshooting steps.

For example, accessing `wine`:

```sh
$ ./affinity-photo-2.6.4.AppImage wine
Usage: wine PROGRAM [ARGUMENTS...]   Run the specified program
       wine --help                   Display this help and exit
       wine --version                Output version information and exit

```

Or `winecfg`:

```sh
$ ./affinity-photo-2.6.4.AppImage wine winecfg
```

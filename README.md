# cryptsetup-helper-mfserver

This is a VERY simple wrapper to help mounting and unmounting encrypted volumes under Arch Linux. Might work on other distros, but it's not tested. 

Feel free to expand the package's functionality if you want, or message me with ideas. Also, if you'd like to package for another distro, please do. 

## Installation

### Arch Linux

Download the latest version of the package, as of now, `cryptsetup-helper-mfserver-1.1-1-any-pkg-tar-xz`. Then install it. 

    pacman -U /path/to/download/dir/cryptsetup-helper-mfserver-1.1-1-any.pkg.tar.xz

### Others

cryptsetup-helper-mfserver hasn't been packaged for any distro except Arch, but it's quite easy to install. Just download `cryptmount` and `cryptumount` and place them in a program folder on your computer, for example `~/.bin/`. Add that folder to your `$PATH` if it's not already there, then it should just run. 

**Please observe** that cryptsetup-helper-mfserver has only been tested on Arch Linux and Debian. 

## Usage

    cryptmount /dev/sdxX name-of-disk

Mounts `/dev/sdxX` on `/run/media/$USER/name-of-disk`. Will prompt you for a password. 

    cryptumount name-of-disk

Unmounts `/run/media/$USER/name-of-disk`. 


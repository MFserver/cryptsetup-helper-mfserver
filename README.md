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

    cryptmount sdxX

Mounts `/dev/sdxX` on `/run/media/$USER/UUID-of-disk`. Also checks in `~/.cryptmount/keys/` for a keyfile correspondng to the UUID of `/dev/sdxX`, and if it exists, it'll use it to mount the disk. If there's no key, it'll prompt for a password, then ask if you want to automatically create a keyfile. 

    cryptumount sdxX

Unmounts `/run/media/$USER/UUID-of-disk`. 

## Pro tip

You can have the keyfile folder synchronized between your computers, and you'll basically never have to worry about a password again. 

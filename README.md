# cryptsetup-helper-mfserver

This is a VERY simple wrapper to help mounting and unmounting encrypted volumes under Arch Linux. Might work on other distros, but it's not tested. 

## Installation

Download the latest version of the package, as of now, `cryptsetup-helper-mfserver-1.1-1-any-pkg-tar-xz`. Then install it. 

    pacman -U /path/to/download/dir/cryptsetup-helper-mfserver-1.1-1-any.pkg.tar.xz

## Usage

    cryptmount /dev/sdxX name-of-disk

Mounts `/dev/sdxX` on `/run/media/$USER/name-of-disk`. Will prompt you for a password. 

    cryptumount name-of-disk

Unmounts `/run/media/$USER/name-of-disk`. 

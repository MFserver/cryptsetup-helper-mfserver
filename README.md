# cryptsetup-helper-mfserver

This is a VERY simple wrapper to help mounting and unmounting encrypted volumes under Arch Linux. Might work on other distros, but it's not tested. 

## Usage

    cryptmount /dev/sdxX name-of-disk

Mounts `/dev/sdxX` on `/run/media/$USER/name-of-disk`. Will prompt you for a password. 

    cryptumount name-of-disk

Unmounts `/run/media/$USER/name-of-disk`. 

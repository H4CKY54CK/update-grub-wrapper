# update-grub-wrapper

"Wrapper" isn't the best word. But the repo is already made. Deal with it.

This script does 2 things. It mounts your unmounted partitions from all drives. Then it runs `update-grub`. Then it unmounts the partitions it mounted in the first step. That means, yes, this script requires `sudo`.

The reason I made this script is because I run into problems when I forget to mount my stuff before running `sudo update-grub`. I then have to use a SIGKILL on the `grub-mount` that is using 100% of one of my CPUs. Hopefully, this will be the end of my `grub-mount` problems.
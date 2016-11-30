## How to mount a VirtualBox shared folder (from a Linux guest)?

* add your share directory in the VirtualBox (e.g. name the shared folder as host_share_folder)

* make a directory on your guset OS for your mount preferably in your home directory (e.g. ~/guest_mount_point)

* open the terminal and mount the shared folder:
```sudo mount -t vboxsf host_share_folder ~/guest_mount_point/```

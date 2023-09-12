Create a unique temporary mount for the `efiboot.img`.

The decision to mount to a unique directory instead of `/mnt` 
is so that multiple jobs can be run simultaneously.
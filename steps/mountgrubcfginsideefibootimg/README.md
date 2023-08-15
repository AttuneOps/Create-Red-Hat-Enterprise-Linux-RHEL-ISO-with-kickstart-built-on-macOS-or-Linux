The unique directory `{ksAttuneBaseDir}/build-{targetServer.fqn}/temporary_mount` is a temporary mount for `images/efiboot.img`.

The decision to mount to a unique directory instead of `/mnt` 
is so that multiple kickstarts can be run simultaneously.
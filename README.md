# archiso-profiles-arkdep

ArchISO configurations used to build Manjaro Immutable netinstaller images.

## Building an image

```bash
cd gnome-arkdep
sudo mkarchiso -v -w workdir/ -o out/ .
```

## Updating the kernel

Due to how Manjaro manages its kernels, updating the kernel images is a manual process.

1. Update the kernel in packages.x86\_64.
1. Update the bootloader entries in `efiboot/loader/`.

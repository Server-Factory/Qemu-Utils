# Server Factory Qemu Utils

Qemu utils for [Server Factory](https://github.com/Server-Factory/Core-Framework).

## Notes

This set of Qemu management scripts is in proof of concept phase. It is not production ready.
So far it has been tried out on macOS only!

Example files for `image_sync.sh`, `image_location.settings` and `image_provider.settings` 
are located under [Examples](./Examples) directory.

## How to use

Tbd.

## Preparing guest operating systems

Guest operating system should be installed with `noapic` setting for the kernel.
To do so follow these steps:

- Boot into the guest operating system
- Edit the following file: `/boot/grub2/grub.cnf`
- Locate kernel loading line ad append `noapic` setting. Line should look similar to this: 
`kernel /vmlinuz-2.6.18-194.el5 ro root=/dev/VolGroup00/LogVol00 rhgb quiet noapic acpi=off`


# magisk-fusermount-bin

Magisk module that installs a `fusermount` binary into `/system/bin`.

I made it for Android setups where tools such as `rclone mount` failed because `fusermount` was missing.

## How It Works

This repo is already laid out as a Magisk module. It ships a prebuilt `system/bin/fusermount` binary plus the metadata and shell hooks needed for Magisk to install it.

The install and boot scripts both make sure the binary keeps executable permissions after installation and across reboots.

## Install

Install it as a Magisk module, then reboot.

## Note

The current binary was sourced from this XDA thread:

- `https://forum.xda-developers.com/t/fusermount-on-android-rclone-mount.3866652/`

## Notes

- Android/Magisk only.
- This repo packages a binary; it does not build `fusermount` from source.

# ansible

Ansible scripts for setting up a test system for Qemu development.

## Role Structure
There are currently three roles:
- packages: Updates and installs some useful packages
- linux: compiles and installs the needed kernel
- qemu: compiles our qemu repo
The linux and qemu roles might become mature enough at some point to justify
an own repo.

## Target
This was written for and tested on a Debian 11 bulleye VM, but should also
work on other Debian-based distros like Ubuntu. Altering this for other
distros should be fairly easy though. There is not much distro-specific
stuff in here except for the usage of APT.

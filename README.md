# ipv6-lab
Data to help you with the IPv6-only home lab

# iPXE
In the iPXE directory, you will find ROM images for VMware network cards (to support legacy BIOS boot over IPv6). You will also find a sample iPXE boot script which will boot Debian-based netboot image.

# Kea
In the `kea-dhcpv6-netboot` directory, there's a sample config for Kea DHCP server to help you with network boot. Supports UEFI HTTP/TFTP iPXE chainloading and iPXE direct boot.

# KVM/UEFI
In the `kvm-qemu-uefi` there is a config for the latest `libvirtd` to load a specific OVMF UEFI binary and variables.
The binaries do boot via IPv6, but iPXE chainloading is currently broken (it used to be working in 2018) and results in getting stuck at `iPXE initialising devices...`.

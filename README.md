# KRIEG-OS

My personal Arch setup I am configuring from scratch to learn more about Linux-based Operating Systems.

- OS: **Arch Linux**
- Firmware interface: **UEFI**
- Boot loader: **GRUB** (integrated with BTRFS for easy snapshot tollback)
- Secure boot: Manually enabled and configured using `sbctl`. 
- Root filesystem: **BTRFS**
- Disk encryption: **LUKS** (integrated with **TPM2** for automatic unlocking).
- Firewall: `ufw` (Uncomplicated Firewall)
- Display Server Protocol: **Wayland**
- Window Compositor: **Hypland**

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

# Dotfiles
The dotfiles for this setup are managed using GNU Stow and can be found in the `dotfiles` directory.
They are organized into subdirectories corresponding to different applications and configurations, making it easy to manage and deploy them across different systems.

> [!NOTE]
> To prevent symlinks of the parent directories, the `--no-folding` option is used when running `stow`. This ensures that only the files within the specified subdirectories are symlinked, rather than the entire directory structure.
> For example, running
> ```bash
> stow --no-folding --target=~ hyprland
> ```
> will create symlinks for the files in the `hyprland` subdirectory without creating a symlink for the `hyprland` directory itself.
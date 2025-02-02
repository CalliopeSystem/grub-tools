# grub-tools
A small collection of tools and related features for grub.

Name | Description
---- | -----------
grub-update-after-kernel.hook | Automatically updates grub.cfg after a kernel is installed/uninstalled.
grub-update-after-ucode.hook | Automatically updates grub.cfg after a microcode is installed/uninstalled.

<br>

## grub-update-after-kernel.hook

This pacman hook automatically updates **/boot/grub/grub.cfg** after a kernel is installed or uninstalled.

## grub-update-after-ucode.hook

This pacman hook automatically updates **/boot/grub/grub.cfg** after a microcode is installed or uninstalled.

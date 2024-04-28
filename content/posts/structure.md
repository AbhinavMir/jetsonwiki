---
title: Structure of the L4T distribution
--- 

What you download in ["preparing your L4T"](/posts/preparing) is not the OS itself, but a suite to help you flash more easily. 

L4T stands for Linux for Tegra, which is a Linux-based software distribution by NVIDIA specifically designed for their Tegra processor-based devices, such as the Jetson embedded computing modules and developer kits.

The file structure you provided is not an OS itself, but rather a collection of files and directories that make up the L4T software distribution. It contains the necessary components to build and flash a complete Linux-based operating system for Tegra devices.

The key components of the L4T distribution include:

1. Bootloader and related files
2. Linux kernel image and modules
3. NVIDIA-specific drivers and libraries
4. Sample filesystem (rootfs) and configuration files
5. Tools and utilities for building, flashing, and customizing the software

When these components are combined and built properly, they create a complete operating system image that can be flashed onto a Tegra device, providing a functional Linux-based environment with hardware-specific optimizations and features.

The provided file system tree represents the structure of the Linux for Tegra (L4T) distribution. Here's an explanation of the main directories and their purposes:

1. `bootloader/`: Contains bootloader-related files such as firmware binaries, configuration files, and scripts for generating boot partitions.

2. `kernel/`: Contains the Linux kernel image, device tree files (`.dtb` and `.dtbo`), and kernel-related packages and modules.

3. `nv_tegra/`: Contains NVIDIA-specific files and packages for Tegra, including BSP (Board Support Package) files, graphics demos, Debian packages, and additional tools.

4. `nv_tools/`: Contains scripts for applying kernel files, customizing the root filesystem, and repackaging the distribution.

5. `rootfs/`: Typically contains the root filesystem image, but in this case, it only has a README file.

6. `source/`: Contains build scripts and Makefiles for building the kernel and other components from source.

7. `tools/`: Contains various tools and utilities for backup/restore, board automation, Debian package handling, disk encryption, and more.

8. `generate_capsule/`: Contains scripts and utilities for generating firmware update capsules (which are used to update firmware on the device).

The top-level directories also include:

- Configuration files for different Jetson boards and variants (e.g., `p3737-0000-p3701-0000.conf`, `p3768-0000-p3767-0000-a0.conf`).
- Flash-related scripts (e.g., `flash.sh`, `nvautoflash.sh`, `l4t_flash_prerequisites.sh`).
- License and agreement files (e.g., `Tegra_Software_License_Agreement-Tegra-Linux.txt`).

The overall structure separates different components of the L4T distribution, such as the bootloader, kernel, NVIDIA-specific files, tools, and configuration files. This organization allows for easy management and customization of the distribution for different Jetson boards and use cases.
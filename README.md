# Kali NetHunter Kernel Builder

## Judyln layout

This repository contains the NetHunter build scripts and patches only.
Clone the kernel source separately and point the builder to it.

Example (sibling directory):

```console
$ git clone <kernel-source-url> ../android_kernel_lge_sdm845
```

If your kernel source is elsewhere, set it in `local.config`:

```bash
KDIR=/path/to/android_kernel_lge_sdm845
KERNEL_DIR=/path/to/android_kernel_lge_sdm845
CONFIG=lineageos_judyln_defconfig
```

## Installation

Clone this repository into your kernel source tree, e.g.

```console
$ cd android_kernel_oneplus_sm8150/
$ git clone https://gitlab.com/kalilinux/nethunter/build-scripts/kali-nethunter-kernel-builder.git
```

**cd** into `kali-nethunter-kernel/`, open `config` and make sure that you are happy with all the settings.

Important: Changes should not be made in this file. Copy it across to `local.config` and delete everything except the parameters you would like to change. Change those parameters and save it.

The settings in `local.config` overwrites `config` but will itself not be overwritten by updates.

# Kali NetHunter Kernel Builder

## English

### Judyln NetHunter Kernel - LG G7 (Judyln)

This repository contains the NetHunter build scripts and patches optimized for the **LG G7 (judyln)** device.
Clone the kernel source separately and point the builder to it.

The build configurations are pre-configured in the scripts to ensure seamless compilation without compatibility issues.

**Clone the LineageOS kernel source:**

```console
$ git clone https://github.com/LineageOS/android_kernel_lge_sdm845.git ../android_kernel_lge_sdm845
```

If your kernel source is elsewhere, set it in `local.config`:

```bash
KDIR=/path/to/android_kernel_lge_sdm845
KERNEL_DIR=/path/to/android_kernel_lge_sdm845
CONFIG=lineageos_judyln_defconfig
ARCH=arm64
CC=clang
```

All patches under `patches/` are currently applied and working correctly.

### Installation

Clone this repository into your kernel source tree, e.g.

```console
$ cd android_kernel_oneplus_sm8150/
$ git clone https://gitlab.com/kalilinux/nethunter/build-scripts/kali-nethunter-kernel-builder.git
```

**cd** into `kali-nethunter-kernel/`, open `config` and make sure that you are happy with all the settings.

Important: Changes should not be made in this file. Copy it across to `local.config` and delete everything except the parameters you would like to change. Change those parameters and save it.

The settings in `local.config` overwrites `config` but will itself not be overwritten by updates.

## Español

### Kernel NetHunter Judyln - LG G7 (Judyln)

Este repositorio contiene los scripts de build y parches de NetHunter optimizados para el dispositivo **LG G7 (judyln)**.
Clona el source del kernel por separado y apunta el builder a ese path.

Las configuraciones de compilación están pre-configuradas en los scripts para garantizar una compilación sin problemas de compatibilidad.

**Clona el source del kernel de LineageOS:**

```console
$ git clone https://github.com/LineageOS/android_kernel_lge_sdm845.git ../android_kernel_lge_sdm845
```

Si tu source está en otro lugar, configúralo en `local.config`:

```bash
KDIR=/path/to/android_kernel_lge_sdm845
KERNEL_DIR=/path/to/android_kernel_lge_sdm845
CONFIG=lineageos_judyln_defconfig
ARCH=arm64
CC=clang
```

Todos los parches en `patches/` están aplicados y funcionando correctamente.

### Instalacion

Clona este repositorio dentro del arbol de tu kernel, por ejemplo:

```console
$ cd android_kernel_oneplus_sm8150/
$ git clone https://gitlab.com/kalilinux/nethunter/build-scripts/kali-nethunter-kernel-builder.git
```

Entra a `kali-nethunter-kernel/`, abre `config` y revisa las opciones.

Importante: no edites `config`. Copialo a `local.config` y deja solo los parametros que quieras cambiar.

Los valores en `local.config` sobrescriben `config` pero no se sobreescriben en futuras actualizaciones.

# Kali NetHunter Kernel Builder

## English

### Judyln layout

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

All patches under `patches/` are currently applied and working.

### Installation

Clone this repository into your kernel source tree, e.g.

```console
$ cd android_kernel_oneplus_sm8150/
$ git clone https://gitlab.com/kalilinux/nethunter/build-scripts/kali-nethunter-kernel-builder.git
```

**cd** into `kali-nethunter-kernel/`, open `config` and make sure that you are happy with all the settings.

Important: Changes should not be made in this file. Copy it across to `local.config` and delete everything except the parameters you would like to change. Change those parameters and save it.

The settings in `local.config` overwrites `config` but will itself not be overwritten by updates.

## Espanol

### Estructura Judyln

Este repositorio contiene solo los scripts de build y parches de NetHunter.
Clona el source del kernel por separado y apunta el builder a ese path.

Ejemplo (directorio hermano):

```console
$ git clone <kernel-source-url> ../android_kernel_lge_sdm845
```

Si tu source esta en otro lugar, configuralo en `local.config`:

```bash
KDIR=/path/to/android_kernel_lge_sdm845
KERNEL_DIR=/path/to/android_kernel_lge_sdm845
CONFIG=lineageos_judyln_defconfig
```

Todos los parches en `patches/` estan aplicados y funcionando.

### Instalacion

Clona este repositorio dentro del arbol de tu kernel, por ejemplo:

```console
$ cd android_kernel_oneplus_sm8150/
$ git clone https://gitlab.com/kalilinux/nethunter/build-scripts/kali-nethunter-kernel-builder.git
```

Entra a `kali-nethunter-kernel/`, abre `config` y revisa las opciones.

Importante: no edites `config`. Copialo a `local.config` y deja solo los parametros que quieras cambiar.

Los valores en `local.config` sobrescriben `config` pero no se sobreescriben en futuras actualizaciones.

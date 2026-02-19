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

### Setup

Clone both repositories as siblings:

```console
$ mkdir -p NetHunter-G7 && cd NetHunter-G7
$ git clone https://github.com/LineageOS/android_kernel_lge_sdm845.git
$ git clone https://github.com/JavierRosas21/NetHunter-Judyln.git kali-nethunter-kernel
```

The build script automatically detects the kernel source. Edit `kali-nethunter-kernel/local.config` only if needed (don't edit `config`). Settings in `local.config` take precedence and persist across updates.

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

### Configuracion

Clona ambos repositorios como directorios hermanos:

```console
$ mkdir -p NetHunter-G7 && cd NetHunter-G7
$ git clone https://github.com/LineageOS/android_kernel_lge_sdm845.git
$ git clone https://github.com/JavierRosas21/NetHunter-Judyln.git kali-nethunter-kernel
```

El script de build detecta automáticamente el source del kernel. Edita `kali-nethunter-kernel/local.config` solo si es necesario (no edites `config`). Los valores en `local.config` tienen prioridad y persisten entre actualizaciones.

---
marp: true
title: Linux rabit hole
theme: default
paginate: true
---
<!-- tema -->
<style>
a[href]{color: #5e81ac;}
section {background: #d8dee9;text-align: justify;color: #3b4252;}
img {background-color: transparent!important;}
img[alt~="center"] {display: block;margin: 0 auto;}
table {text-align: center; margin-left: auto; margin-right: auto;} 
th { background-color: #81a1c1; color: #e5e9f0}
td { background-color: #e5e9f0;}
mark {background-color: rgb(129 161 193 / 0.3)};
h1 {color: #81a1c1;}
h1 strong {color: #4c566a;}
h2 {color: #81a1c1;}
</style>

<!-- HTML Enabled in Marp Markdown-->

![bg opacity:.3](https://c4.wallpaperflare.com/wallpaper/750/507/586/computers-linux-wallpaper-preview.jpg)

<style scoped>h1, h2, h3 {color: #3b4252;}</style>

# <!--fit--> Instalacion de Linux
## Por Ariel Parra.
---


# Medio de instalacion

Recomiendo usar USB 2.0 de maximo 32GB para poder usar fat32 con computadoras antiguas (solo BIOS), para las computadoras modernas no deberia haber problemas.

- [Rufus](https://rufus.ie/): Es para Windows e instala un solo iso

- [Ventoy](https://www.ventoy.net/en/download.html): Es multisistema, la USB se formatea a fat32 o vfat, puedes usar multiples ISOs pasandolos a la USB como si fuese una USB regular

---

# Descarga del dicso de instalacion ISO

Recomiendo Buscar la forma de descargarlo con torrents con la apliacion de [qBitorrent](https://sourceforge.net/projects/qbittorrent/) a travez de repositorios como:

- [fosstorrents](https://fosstorrents.com/distributions/)
- [bitorrent](https://distrowatch.com/dwres.php?resource=bittorrent)
- [linux tracker](https://linuxtracker.org/)

---

# Dualboot con Windows

- De preferencia hacer una Instalacion limpia de Windows.
- Correr el Script De Chris Titus [WinUtil](https://github.com/ChrisTitusTech/winutil).
- Con el script cambiar el tiempo a UTC.
- Hay que modificar el espacio usado de Windows con [diskpart](https://www.howtogeek.com/212/resize-a-partition-on-windows/).
- Hay que poner Windows en [modo seguro](https://support.microsoft.com/en-us/windows/start-your-pc-in-safe-mode-in-windows-92c27cff-db89-8644-1ce4-b3e5e56fe234) antes de moverle a la BIOS/UEFI.
- Hay que desactivar el [arranque rapido](https://www.howtogeek.com/856514/how-to-disable-fast-startup-on-windows-10/).
- Hay que desactivar la hibernacion con CMD
```
powercfg.exe /hibernate off
```
- Si se ocupa RAID poner este comando en CMD
```
bcdedit /set safeboot minimal
```

---  

# Dualboot con MacOSX

- Para computadoras Mac con Procesadores Intel (x64)
[Guia por makeuseof](https://www.makeuseof.com/tag/install-linux-macbook-pro/)

- Para computadoras Mac con procesadores M1/M2 (arm)
[Asahi Linux](https://asahilinux.org/2022/03/asahi-linux-alpha-release/) o [Fedora Asahi Remix](https://fedora-asahi-remix.org/)


---
   
# BIOS/UEFI

- Hay que activar el arranque por USB (boot from USB/ Boot order)
- Hay que desactivar el secure boot
- Si tienes NVME/mSATA recomiendo AHCI en lugar de RAID
- En casos especificos de UEFI tienes que activar legacy boot/BIOS

---

# Tipos de Instalacion
![bg opacity:.3](https://preciogas.com/sites/preciogas.com/files/styles/_default/public/images/precio-instalacion-825x293.png)

---   

# Instalacion copiando el RootFs

- [Arch](https://wiki.archlinux.org/title/Installation_guide): Es el mas popular, te deja configurar muchas cosas y tambien permite el uso de [arch install scripts](https://github.com/archlinux/arch-install-scripts), solo que este sistema es solo para sistemas x64 (64 bits).

- [Void](https://docs.voidlinux.org/installation/index.html): Es mi recomendacion ligera y rapida para sistemas x86 (32 bits).

- [Gentoo](https://wiki.gentoo.org/wiki/Handbook:AMD64): Este es mi opcion recomendada para aprender sobre linux, sus componentes, aplicaciones y tambien sobre compilacion de archivos.


---

# Instalacion con una herramienta para SBC

- [Balena Etcher](https://etcher.balena.io/): Sirve para ISOs y para .xz (formato usado para SBCs).

- [USB Imager](https://gitlab.com/bztsrc/usbimager): Mi recomendacion personal.

- [Raspberry Pi Imager](https://www.raspberrypi.com/software/): Es software de Raspberry Pi para Raspberry Pis

---

# Instalacion a partir de Calamares

![bg opacity:.3](https://calamares.io/images/2020/arco_welcome.webp)

---

![center](https://www.zdnet.com/a/img/2016/06/08/0b3b2d13-7984-4db6-a7bb-4bfe50199e91/welcome.png)

---

![center](https://www.zdnet.com/a/img/2016/06/08/0de2cedc-eab0-4f84-9336-5f1b10404b4e/timezone.png)

---

![center](https://www.zdnet.com/a/img/2016/06/08/413e4859-0bff-494f-909b-5ce7c22b934f/keyboard.png)

---

![center](https://www.zdnet.com/a/img/2016/06/08/c4d66700-db89-4a07-b925-b22cb4871de4/partition.png)

---

![center](https://www.zdnet.com/a/img/2016/06/08/2a50f01d-cf2d-40b5-9fac-c2f47c94dc15/userinfo.png)

---


![center](https://www.zdnet.com/a/img/2016/06/08/a4d0c875-0de0-4d4b-bc5d-20b8da365ef2/summary.png)

---

![center](https://www.zdnet.com/a/img/2016/06/08/0246146c-e0fa-4cc3-aa04-a2843a3223ac/installing.png)

---

![center](https://www.zdnet.com/a/img/2016/06/08/5c37ee02-eb9f-49a7-8025-64e60786e1e8/complete.png)

---

# Particiones

![bg opacity:.3](https://i.guim.co.uk/img/media/9d43b48e8e83ec78c24b04eaee7a87574b7a4883/0_181_5195_3118/master/5195.jpg?width=1200&quality=85&auto=format&fit=max&s=c0464dce767b7b0b1478f9d85632882a)

---

Es la designacion de espacio en disco para los sitemas operativos y particiones de servicio, esto usualmente se hace atravez de un live iso, con la aplicacion de gparted
![center](https://gparted.org/screens/gparted-main-window.png)

---


## Tablas de particion

- MBR: limitado a 4 particiones y 2 TB de espacio para legacy BIOS, Usado por Windows antiguos

- GPT: particiones, subparticiones y tamano ilimitado

## RootFs

Es donde se encuentra el sistema operativo y las carpetas de usuario, este se indica con la direccion "/".

---

## Formatos de archivos

Windows usa NTFS y para acceder para escribir desde Linux ocupas NTFS3G 

El formato de archivos mas rapido y eficiente para escritorios es ext4

El formato mas moderno con mas funciones es btrfs este viene incluido en Fedora, este es util para hacer respaldos automaticos con timeshift.

## Swap

Tambien conocido como espacio de memoria Virtual, es un espacio en disco con formato swapfs, designado de desbordamiento cuando la memoria principal RAM se llena. Este mejora la eficiencia del sistema, lo mas comu suele ser usar 4GB

---

# Eleccion de Inicio de Sistemas

- BIOS/UEFI: Muchas BIOS/UEFI tienen la opcion de elegir el sistema operativo. 

- [GRUB + GRUB OS prober](https://wiki.archlinux.org/title/GRUB#Detecting_other_operating_systems): este se configura dentro de Linux editando el archivo /etc/default/grub, quitando el comentario de la linea:
```
#GRUB_DISABLE_OS_PROBER=false       ->     GRUB_DISABLE_OS_PROBER=false 
```

---

# Referencias 

- https://askubuntu.com/questions/963087/install-dual-boot-ubuntu-with-windows-10-and-raid-on
- https://www.makeuseof.com/tag/install-linux-macbook-pro/
- https://learn.microsoft.com/en-us/windows-server/storage/disk-management/shrink-a-basic-volume
- https://wiki.archlinux.org/title/Dual_boot_with_Windows
- https://learn.microsoft.com/en-us/troubleshoot/windows-client/deployment/disable-and-re-enable-hibernation
- https://calamares.io/docs/users-guide/

---

- https://learn.microsoft.com/en-us/windows-server/storage/disk-management/change-an-mbr-disk-into-a-gpt-disk
- https://www.makeuseof.com/mount-ntfs-windows-drives-in-linux/
- https://wiki.archlinux.org/title/Swap
- https://learn.microsoft.com/en-us/linux/install
- https://www.zdnet.com/article/hands-on-with-ubiquity-and-calamares-two-linux-installers-side-by-side/

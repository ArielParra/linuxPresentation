---
marp: true
title: linux rabit hole
theme: default
paginate: true
---

![bg opacity](rabithole.png)
# <!--fit--> linux rabit hole
## curso completo de linux y los temas que lo rodean
### por Ariel Parra

---

# Contenidos
<style scoped>
ol{ columns: 2; }
</style>
1. ¿Qué es Linux?   
1.1 Definición
1.2 Historia
1.3 Distribuciones
2. sistemas operativos
2.1 porque usar linux
2.2 problemas de windows
3.
4.
5.
6.
7.  
8.
9.
10.


---

# **1. ¿Qué es linux?**

---

# 1.1 Definición
Es un kernel monolitico de codigo abierto con licencia GNU GPL v2.<br>

---

- que es un kernel monolitico? El kernel es un software que tiene el control del hardware, administra y optimiza los recursos del sistema como alocacion de memoria ram, procesos del CPU, drivers, etc. Actuando asi como un puente entre aplicaciones y el hardware. Este es monolitico cuando todos los servicios del sistema operan en el kernel atravez de system calls   
- que es el codgo abierto? Es software donde cualquier persona puede ver,analizar y por ende modificar el codigo fuente
- cual es la licencia GPLv2?  Es una licencia de software donde cualquier modificacion al codigo debe tener la misma licencia y tambien que por cada archivo binario que sea distribuido tiene que estar disponible su codigo fuente.

---

# 1.2 Historia 

Fue creado en 1991 por el estudiante de la universidad de Helsinki Linus Torvalds, al mismo tiempo Richard Stallman junto con su proyecto GNU de la fundacion de software libre (FSF) ya habian creado las aplicaciones y utilidades de un sistema operativo. Estas aplicaciones y utilidades fueron agregadas al Linux kernel para crear un systema completo llamado GNU/Linux

---

# **diagrama de abrir mi pagina web**

bios -> bootloader -> linux kernel -> PID1 (init system) ->  login manager tty/ssdm -> DE -> chromium -> pagina web

---

# **Desventajas de windows**
un chingo, creanme

---

# dev
referencia [1](#referncias)

- java updater, javahome path
- ejecuta programas de manera lenta en la terminal aunque sea pwsh
- virtualizacion rompe elementos del sistema dell alienware control / throttle stop
- para el android studio, intel HAXM interfiere con hyper V 
- al moverle al los hosts dejo de funcionar el internet 
- al compilar sueles ocupar windows SDKs y solo se consiguen descargando visual studio community
- visual studio community usa como 10gb o mas incluyendo temp files
- problemas con librerias, aveces tienes que compilarlas manualmente como pyucripto

---

# privacidad
windows calls home.
los botones de privacidad estan activados por defecto
no solo windows sino edge y office
app acces to user information
Delivery Optimization 

---

# uso
en windows te obliga a tener una cuenta microsoft y usarla en tu sistema    
el sistema se expande, el puro sistema operativo ocupa masomenos 40gb base pero se expande con uso como 15gb
la busqueda de archivos especificos tarda mucho
las aplicaciones se actualizan individualmente, no puedes regresar a una version anterior
existe winget pero tienes que tener cuenta microsoft y aceptar las condiciones y aun asi no tiene todo el software
aplicaciones de utilidades freeware pueden tener virus como atubecatcher, etc.
la microsoft store tiene aplicaciones más aplicacioens .appx que .exe
tienes que pagar para poder ver fotos heic
windows oem bloatware

---

antivirus sirven pa pura verga y te bloquean los firewall y usan mas recursos de lo normal
high dpi scaling is messed up (blurry apps)
permisos en carpetas de sistema limitados
no puedes parar las actulizaciones o solo elegir ciertas actulizaciones sin moverle al regedit
la solucion a la mayoria de errores es reistalar el sistema operativo
las nuevas apps crean servicios que se ejecutan al inicio que no se desactivan si no es que te metes a services/regedit

---

# hardware
si quieres drivers actualizados tienes que buscarlos en internet
los discos duros tienen que defragmentarse con el file sistem ntfs
los drivers the nvidia tienen telemetria

# juegos
descargas cada version inimaginable de microsoft visual c++ redistributable
en las apps de xbox/mstore no te deja acceder a los archivos del juego sin moverle a los permisos

# customize
wallpaper engine 50 pesos en steam


---

# **linux distributions**

---

que son, quien sabe
las distribuciones se pueden diferenciar por tres partes principales:
el sistema de arranque (init system (PID 1)), gestor de paquetes (package manager) 
y su filosofia (uso,caracteristicas,orientacion,etc.)

---

<style scoped>table {font-size: 28px;}</style>

| distribucion | init           | pkg manager | filosofia    |
|--------------|----------------|-------------|--------------|
| alpine       | openrc         | apk         | no gnu       |
| arch         | systemd        | pacman      | bleeding edge|
| debian       | systemd        | apt         | community    |
| Slackware    | sysV           | slackpkg    | kiss         |
| SUSE LE      | systemd        | zipper      | enterprise   |
| gentoo       | openrc/systemd | portage     | compile      |
| void         | runit          | xbps        | BSD-feel     |
| nixos        | systemd        | nix         | portability  |
| RHEL         | systemd        | yum         | enterprise   |

---

<style scoped>table {font-size: 28px;}</style>

# deribadas



| distribucion | init             | basado en   | filosofia 
|--------------|------------------|-------------|-----------
| artix        | runit/openrc/etc | arch        | no systemd
| devuan       | openrc           | debian      | no systemd
| Ubuntu       | systemd          | debian      | enterprise
| Uaabuntu     | systemd          | ubuntu      | educacion
| openSUSE     | systemd          | SUSE        | community
| parabola     | runit/openrc/etc | arch        | no systemd
| Fedora       | systemd          | RHEL        | comunitty

---

# Referencias

---

# 1. Que es linux

---

<style scoped>{font-size: 21px;}</style>

# 1.1
- GeeksforGeeks. (2019). *Linux Tutorials | Getting Started | Introduction | GeeksforGeeks*. https://yewtu.be/watch?v=0EDwEQoui_g
- GNU. (2023). *GNU General Public License, version 2*. https://www.gnu.org/licenses/old-licenses/gpl-2.0.html
- Opensource.com. (s.f.). *What is Linux?*. https://opensource.com/resources/linux
- Opensource.com. (s.f). *What is open source?*.https://opensource.com/resources/what-open-source
- Open Source Initiative. (2007). *The Open Source Definition*. https://opensource.org/osd/
- Red Hat. (2019). *What is the Linux kernel?*. https://www.redhat.com/en/topics/linux/what-is-the-linux-kernel 
- Roch, B. (2004). *Monolithic kernel vs. Microkernel*. https://web.cs.wpi.edu/~cs3013/c12/Papers/Roch_Microkernels.pdf 
- The Linux Kernel Organization. (2019). *Is Linux Kernel Free Software?*. https://www.kernel.org/category/faq.html

---

<style scoped>{font-size: 21px;}</style>

# 1.2 
- Britannica, T. Editors of Encyclopaedia (2023). *Linux*. Encyclopedia Britannica. https://www.britannica.com/technology/Linux
- Fireship. (2022). *Linux in 100 Seconds* [Video]. YouTube. https://yewtu.be/watch?v=rrB13utjYV4
- The Linux Information Project. (2006). *What is Linux?*. http://www.linfo.org/newbies.html
- The Linux Kernel Organization. (2019). *About Linux Kernel*. https://www.kernel.org/linux.html
- Wheeler, D. (2003). *History of Unix, Linux, and Open Source / Free Software*. https://tldp.org/HOWTO/Secure-Programs-HOWTO/history.html

---
# linux distributions

*filosofia o descripcion por sistema :v*
https://docs.slackware.com/slackware:philosophy

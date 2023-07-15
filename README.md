---
marp: true
title: 03 May 2021
theme: default
paginate: true
---

# **linux rabithole**
## **curso completo de linux y los temas que le rodean**
### por Ariel Parra
---

# Contenidos
1.¿Qué es Linux?
2.
3.
4.
5.

---

# **1. ¿Qué es linux?**

---

es un kernel

---

# **distros**

---
| distribucion | init             | pkg manager | basado |
|--------------|------------------|-------------|--------|
| arch         | systemd          | pacman      | no     |
| artix        | runit/openrc/etc | pacman      | arch   |
| gentoo       | openrc/systemd   | portage     | no     |
| debian       | systemd          | apt         | no     |
| devuan       | openrc           | apt         | debian |
| suse         | systemd          | yum         | no     |



---

# **Desventajas de windows**

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

# referencias

---
# 1. Que es linux
Britannica, T. Editors of Encyclopaedia (2023, May 15). *Linux*. Encyclopedia Britannica. https://www.britannica.com/technology/Linux
The Linux Kernel Organization. (2019, September 20). *About Linux Kernel*. https://www.kernel.org/linux.html
Opensource.com. (n.d). *What is Linux?*. https://opensource.com/resources/linux
Fireship. (2022, March 11). *Linux in 100 Seconds* [Video]. YouTube. https://yewtu.be/watch?v=rrB13utjYV4

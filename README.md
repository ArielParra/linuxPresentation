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
# aunque antes tendria que hablar de distros y  tambien que los compone
# 1.3 Filosofias relacionadas

Free/libre opensource software
Privacy concerns
posix

minimalism/anti bloat
    anti gnu
    anti systemd

---

# 1.4 ventajas o pq usarlo
el audio es mejor con pipewire 
rapidez de boot
rapidez de compilacion
rapidez de ejecucion
estabilidad
comuninidad 
etc et
 
---

# **Desventajas de windows**

---

# Desarrollador
- [java updater](https://www.java.com/en/download/help/java_update.html) esta siempre activo en segundo plano
- ejecuta programas de manera lenta (a tirones) aunque sea pwsh
- [.NET](https://michaelscodingspot.com/dotnet-dll-hell/) y [dll](https://www.partech.nl/en/publications/2022/03/what-is-dll-hell-problem-and-how-to-solve-it) [hell](https://www.baeldung.com/cs/dll-hell-problem)
- Hyper-V solo esta disponible para [Windows Pro](https://www.microsoft.com/en-us/windows/compare-windows-10-home-vs-pro)
- Virtual Machine Platform, Hyper-V, Windows hypervisor platform y WSL2 interfieren con aplicaciones: [dell alienware control](https://www.dell.com/community/Alienware-Desktops/AWCC-OC-Controls-incompatible-with-Virtual-Machine-Platform/m-p/8239494#M60811), [throttle stop](https://www.techpowerup.com/forums/threads/throttlestop-dead-on-windows-11.284102/), etc.
- los hosts en windows son [read-only](https://superuser.com/questions/958991/windows-10-cant-edit-hosts-file) 
- para correr un [hello world!](https://stackoverflow.com/questions/55603111/unable-to-compile-rust-hello-world-on-windows-linker-link-exe-not-found) de rust ocupas que descargar visual studio community junto con 1gb para los c++ build tools y el Windows SDK 
- visual studio community usa como [10gb](https://developercommunity.visualstudio.com/t/visual-studio-uses-too-disk-much-space/145475) o [más](https://developercommunity.visualstudio.com/t/hard-disk-space-loss/585904)
- problemas con librerias, aveces tienes que compilarlas manualmente como [pycripto](https://old.reddit.com/r/webdev/comments/132eql/owhy_many_people_dislike_windows_as_an_development/) o en mi caso librespot de rust 
---

# uso
- las apps por defecto se actualizan individualmente ya sea abriendo la aplicación o teniendo que descargar la nueva version de la pagina del creador

- para usar winget ocupas una cuenta microsoft para descargar [App-Installer](https://apps.microsoft.com/store/detail/appinstaller/9NBLGGH4NNS1?hl=de-at&gl=at&rtc=1) de la microsoft store y para usarlo ocupas constantemente aceptar los [UAC](https://learn.microsoft.com/en-us/windows/package-manager/winget/) prompts, aparte de acepatar la [CLA](https://opensource.microsoft.com/cla/) 

- no puedes nombrar archivos con ciertos [nombres](https://yewtu.be/watch?v=bC6tngl0PTI)
- windows pro cuesta [$6399](https://www.microsoft.com/es-mx/d/windows-11-pro/dg7gmgf0d8h4) pesos MXN
- windows 11 te obliga a tener una cuenta microsoft y usarla en tu sistema
- el sistema se expande, el puro sistema operativo ocupa masomenos 40gb base pero se  expande con uso como 15gb
- el buscador de windows es [ineficiente](https://computerinfobits.com/why-is-windows-10-search-so-bad/)
- prefetch y superfetch (SysMain), suelen tener el disco duro al [100%](https://yewtu.be/watch?v=MmH4tjH2yMc) de uso 

---

- aplicaciones freeware pueden tener virus como [atubecatcher](https://old.reddit.com/r/antivirus/comments/snqipr/is_atube_catcher_a_virus/), etc.
- la microsoft store tiene aplicaciones más aplicacioens [.appx](https://learn.microsoft.com/en-us/uwp/schemas/appxpackage/uapmanifestschema/schema-root
) que .exe
- tienes que pagar para poder usar archivos [HEVC](https://apps.microsoft.com/store/detail/hevc-video-extensions/9NMZLZ57R3T7?hl=en-us&gl=us&activetab=pivot%3Aoverviewtab)
- windows incluye [bloatware](https://www.digitalcitizen.life/windows-10-bloatware/)
- antivirus pueden bloquear aplicaciones/servicios en el [firewall](https://www.mcafee.com/support/?locale=en-US&articleId=TS102946&page=shell&shell=article-view) 
- Windows Antimalware Service puede usar [100%](https://answers.microsoft.com/en-us/windows/forum/all/high-cpu-usage-by-antimalware-service-executable/4f6f635a-b3ad-444c-8cd0-68fb1e9f4bfa) del cpu
- Problemas en pantallas con [high dpi](https://support.microsoft.com/en-gb/topic/windows-scaling-issues-for-high-dpi-devices-508483cd-7c59-0d08-12b0-960b99aa347d) dando lugar a [apps borrosas](https://support.microsoft.com/en-us/windows/fix-apps-that-appear-blurry-in-windows-10-e9fe34ab-e7e7-bc6f-6695-cb169b51de0f)
- la solucion a la mayoria de errores es [reistalar](https://answers.microsoft.com/en-us/windows/forum/all/windows-update-system-restore-and-repair-failed/aaf28405-55c0-4ee2-b4b4-f13571680b32) el sistema operativo
- las [apps](https://www.pcmag.com/how-to/stop-windows-10-apps-from-launching-at-startup) se ejecutan al inicio o crean servicios que se ejecutan al inicio
- fondos de pantalla en slidehow puede no [funcionar](https://answers.microsoft.com/en-us/windows/forum/all/background-slideshow-stops-working/acfcabe4-56fb-436a-afc6-42bdd877ca29)
- pocas opciones open source de customizacion [ModernFlyouts](https://github.com/ModernFlyouts-Community/ModernFlyouts), [rainmeter](https://github.com/rainmeter/rainmeter), [RoundedTB](https://github.com/Erisa/RoundedTB),etc.
- algunas opciones de customizacion cuestan [wallpaperengine](https://store.steampowered.com/app/431960/Wallpaper_Engine/), [taskbarX](https://apps.microsoft.com/store/detail/taskbarx/9PCMZ6BXK8GH?hl=en-us&gl=us), [start11](https://www.stardock.com/products/start11/), etc.

---

# hardware
- Device encryption Requires modern hardware (InstantGo/AOAC/HSTI-compliant).
- TPM, requicito para windows 11, bitlocker
- los discos duros con ntfs tienen que [defragmentarse](https://learn.microsoft.com/en-us/previous-versions/cc767961(v=technet.10))
- windows automaticamente desfragmenta los ssd dañando su vita util
- los drivers oficiales de nvidia tienen [telemetria](https://www.geeks3d.com/20161107/nvidia-telemetry-in-geforce-drivers/), la alternativa es usar [nvcleaninstall](https://www.techpowerup.com/download/techpowerup-nvcleanstall/) de techpowerup

---

# juegos
- descargas [muchas versiones](https://www.howtogeek.com/256245/why-are-there-so-many-microsoft-visual-c-redistributables-installed-on-my-pc/) de microsoft visual c++ redistributable por cada juego, una solucion es descargar todos desde [techpowerup](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)
- los juegos de la microsoft store (xbox app) suelen correr [peor](https://old.reddit.com/r/techsupport/comments/v4nhaf/so_ive_been_wondering_if_its_just_me_or_windows/) y dar [input lag](https://www.reddit.com/r/roblox/comments/oahvsf/roblox_player_vs_microsoft_store_app_input_lag/)
- no puedes acceder a las [carpetas](https://www.makeuseof.com/windows-access-windowsapps-folder/) de juegos de la microsoft store (xbox app) aun siendo administrador


---

# privacidad
- windows [phone home](https://yewtu.be/watch?v=IT4vDfA_4NI).
- windows hace backdoors para [NSA](http://techrights.org/wiki/index.php/Microsoft_and_the_NSA) y esta involucrado con [PRISM](https://en.wikipedia.org/wiki/PRISM)
- datos de diagnosticos [obligatorios](https://learn.microsoft.com/en-us/windows/privacy/required-windows-diagnostic-data-events-and-fields-2004)
- [edge](https://learn.microsoft.com/en-us/microsoft-edge/privacy-whitepaper/) y [office](https://learn.microsoft.com/en-us/deployoffice/compat/data-that-the-telemetry-agent-collects-in-office) envian telemetria
- [Delivery Optimization](https://learn.microsoft.com/en-us/windows/deployment/do/waas-delivery-optimization) esta activado por [defecto](https://www.dell.com/support/kbdoc/es-mx/000125580/information-on-the-windows-update-delivery-optimization-feature-within-windows-10?lang=en)

---

# mas lecturas
https://old.reddit.com/r/webdev/comments/132eql/why_many_people_dislike_windows_as_an_development/
https://old.reddit.com/r/linuxmasterrace/comments/u19uee/what_is_your_worst_experience_with_ms_windows/
https://en.wikipedia.org/wiki/Criticism_of_Microsoft
https://wiki.installgentoo.com/wiki/Windows
https://wiki.installgentoo.com/wiki/Windows_10
https://itvision.altervista.org/why-windows-10-sucks.html

---

# ok tienes que usar windows
razones: juegos, photoshop,flvstudio, ms office ,etc
recomendaciones:
scoop como package manager
usalo en una vm con NAT
nvclean install
usa christitus debloat
bloquea hosts
shut up windows 10 ++
desactiva antivirus 
autoruns para desactivar apps/servicios al inicio del sistema 


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

# linux avanzado
sistema jerarquia 
componentes
todos son archivos

---

# Referencias

---

<style scoped>{font-size: 21px;}</style>

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

- Britannica, T. Editors of Encyclopaedia (2023). *Linux*. Encyclopedia Britannica. https://www.britannica.com/technology/Linux
- Fireship. (2022). *Linux in 100 Seconds* [Video]. YouTube. https://yewtu.be/watch?v=rrB13utjYV4
- The Linux Information Project. (2006). *What is Linux?*. http://www.linfo.org/newbies.html
- The Linux Kernel Organization. (2019). *About Linux Kernel*. https://www.kernel.org/linux.html
- Wheeler, D. (2003). *History of Unix, Linux, and Open Source / Free Software*. https://tldp.org/HOWTO/Secure-Programs-HOWTO/history.html

---


*filosofia o descripcion por sistema :v*
https://docs.slackware.com/slackware:philosophy



https://privacy.microsoft.com/en-us/privacystatement
- Jody Bruchon Tech . *Windows 11 Must Be Stopped - A Veteran PC Repair Shop Owner's Dire Warning - Jody Bruchon* [Video]. https://yewtu.be/watch?v=LcafzHL8iBQ

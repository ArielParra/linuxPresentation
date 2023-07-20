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
3. Linux avanzado
3.1 directorios
3.2 bla bla
4. usando linux
4.1 comandos



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
seguridad selinux hardenkernel
minimalism/anti bloat
    anti gnu
    anti systemd

# temas relacionados

# posix   

# Privacy 

avoid honey pots
duckduckgo
starpage
[proton](https://techcrunch.com/2021/09/06/protonmail-logged-ip-address-of-french-activist-after-order-by-swiss-authorities/)

# freeBSD 
es un proyecto ["grande"](https://svnweb.freebsd.org/base/stable/12/) con muchos sistemas operativos forkeados de el

# openBSD
es un proyecto relativamente mas ["chico"](https://cvsweb.openbsd.org/src/) que freebsd 
es [inovador](https://www.openbsd.org/innovations.html
), crean nuevas herramientas usadas en toda la comunidad de unix

ambos pueden tener incompatibilidades de hardware
ambos pueden tener algunas incompatibilidades de software, pero hay capas traduccion y emulacion para solucionarlo




---

# 1.4 ventajas de linux
- es gratuito
- superioridad en cuestion de audio con [pipewire](https://pipewire.org/)
- puede arrancar [rapidamente](https://www.forbes.com/sites/jasonevangelho/2019/06/19/infographics-linux-mint-challenges-windows-10-in-small-business-speed-tests-laptop/#7a560d2369bb) el sistema y las aplicaciones
- tiempos menores de [compilacion](https://medium.com/aedm/windows-wsl-and-linux-a-build-time-benchmark-for-java-rust-go-and-node-43188a9c77d6)
- mejores resultados en [geekbench](https://yewtu.be/watch?v=7BreeFlhP78)
- usa menos memoria [RAM](https://yewtu.be/watch?v=L3d9okxKcjM)
- estabilidad
- tiene multiples [comunidades](https://www.makeuseof.com/tag/4-helpful-communities-new-linux-users/) para soporte
- altamente [customizable](https://www.reddit.com/r/unixporn/)
- tiene drivers opensource oficiales de [AMD](https://gpuopen.com/amd-open-source-driver-for-vulkan/) y no oficiales de [nVidia](https://nouveau.freedesktop.org/)
- puedes [revivir](https://itsfoss.com/mystory-linux-13-years-laptop/) laptops antiguas
- promueve [open source](https://www.linuxfoundation.org/resources/open-source-guides/participating-in-open-source-communities)

----

# más referencias de las ventajas de linux 
- [linfo: 25 Reasons to Convert to Linux](http://www.linfo.org/reasons_to_convert.html)
- [Joe Collins: Linux vs. Windows | The Fundamental Differences](https://yewtu.be/watch?v=p4xA7GRmf6o)
- [Dave's Garage: Linux vs Windows Round 1: Open Source vs Proprietary - From a Retired Microsoft Dev](https://yewtu.be/watch?v=a9ZADRy5W0c)
- [DistroTube: How Linux Respects Your Privacy (And How Windows Does NOT!)](https://yewtu.be/watch?v=KarYADRAoTU)
- [Average Linux User: Linux advantages](https://yewtu.be/watch?v=mJEWPqHXNzs)


---
# desventajas de linux

- tienes que aprender temas nuevos, aprender a buscar soluciones y leer.
- no puedes correr ciertos juegos: [rainbow six](https://www.protondb.com/app/359550), [roblox](https://news.itsfoss.com/roblox-linux-end/), [etc.](https://www.protondb.com/explore?sort=fixWanted)
- no puedes correr ciertas aplicaciones: [Adobe Photoshop](https://appdb.winehq.org/objectManager.php?sClass=application&iId=17), [MS Office](https://appdb.winehq.org/objectManager.php?sClass=application&iId=31), [etc](https://appdb.winehq.org/).
- sin soporte completo para [HDR](https://wiki.archlinux.org/title/HDR_monitor_support) 
- problemas con [impresoras](https://opensource.com/article/21/8/add-printer-linux)
- screen tearing en [X11 (xorg)](https://christitus.com/fix-screen-tearing-linux/) 
- problemas al compartir pantalla con audio en [discord](https://wiki.archlinux.org/title/Discord#Screen_sharing_with_audio) y [MS Teams](https://answers.microsoft.com/en-us/msteams/forum/all/sharing-system-sound-in-teams-for-linux/f1c70d83-e9bd-41b4-abde-d78fae764d5c)
- el driver para nvidia nouveau tiene un [peor rendimiento](https://openbenchmarking.org/result/2106300-IB-NOUVEAU2060) que el oficial
- la capa de compatibilidad con windows wine puede correr [malware](https://wiki.winehq.org/FAQ#Is_Wine_malware-compatible.3F)


---

# ventajas MacOS

- tiene interfaces con diseños [inovadores](https://design.tutsplus.com/tutorials/how-apple-ended-up-leading-the-icon-design-trends-and-whether-or-not-you-should-fight-it--cms-32201)
- tiene una certificacion [posix](https://www.opengroup.org/openbrand/register/apple.htm)
- usar [xcode](https://developer.apple.com/xcode/) para desarrollar aplicaciones de iOS/MacOS
- juegos nativos como [roblox](https://www.roblox.com/download) o juegos de Blizzard como [WOW](https://www.blizzard.com/en-sg/download?platform=macos)
- aplicaciones nativas como [Adobe Photoshop](https://helpx.adobe.com/support/photoshop.html), [MS Office](https://www.microsoft.com/en-us/microsoft-365/mac/microsoft-365-for-mac), [FL Studio](https://www.image-line.com/), etc.
- compatibilidad y uso de [heic/hecv](https://support.apple.com/en-us/HT207022) integrado al sistema
- tienen el [ecosistema de apple](https://www.apple.com/macos/continuity/)
- tienen de los mejores [procesadores arm](https://www.techspot.com/review/2499-apple-m2/) para escritorio
- soporte de [HDR](https://support.apple.com/en-us/HT210980)
- puedes compartir pantalla con sonido en discord y [MS Teams](https://answers.microsoft.com/en-us/msteams/forum/all/sharing-system-sound-in-teams-for-linux/f1c70d83-e9bd-41b4-abde-d78fae764d5c)
- el driver opensource de nvidia novoue rinde peor que el p

---

# desventajas MacOS

- no puede correr ciertos [juegos](https://www.protondb.com/explore?sort=fixWanted)
- quitaron el soporte de [32-bits](https://support.apple.com/en-us/HT208436)
- no puede correr ciertas [apps](https://gist.github.com/stevemoser/a4388df17633beae5bc3fb07d38373e2)
- hardware [oficial](https://everymac.com/systems/apple/index-apple-specs-applespec.html) y [no oficial](https://hackintosh.com/#hackintosh_compatible) limitados
- Appple ID es un requisito para instalar MacOS
- las computadoras Mac son [costosas](https://everymac.com/global-mac-prices/mac-prices-mexico-mx.html)
- la existencia de [OCSP](https://blog.jacopo.io/en/post/apple-ocsp/)
- multiples problemas de [privacidad](https://sneak.berlin/20201112/your-computer-isnt-yours/)
- los [contratos de licencia de software](https://www.apple.com/legal/sla/)
- posibles conexiones con NSA e implicacion con [PRISM](https://www.washingtonpost.com/investigations/us-intelligence-mining-data-from-nine-us-internet-companies-in-broad-secret-program/013/06/06/3a0c0da8-cebf-11e2-8845-d970ccb04497_story.html)
- no suele haber drivers opensource
- la capa de compatibilidad con windows wine puede correr [malware](https://wiki.winehq.org/FAQ#Is_Wine_malware-compatible.3F)

---

# Recomendaciones si tienes que usar MacOS
- no uses una cuenta de Apple ID con tus datos personales
- usa macOS en una vm con NAT activado
- lee esta [guia](https://github.com/drduh/macOS-Security-and-Privacy-Guide) de privacidad
- usa [brew](https://brew.sh/) como package manager


---

# ventajas de windows
- compatibilidad perfecta con [directX](https://www.microsoft.com/en-us/download/details.aspx?id=35)
- [compatibilidad](https://support.microsoft.com/en-us/windows/make-older-apps-or-programs-compatible-with-windows-783d6dd7-b439-bdb0-0490-54eea0f45938) con aplicaciones antiguas de windows
- las empresas les importa la distribucion del [mercado](https://gs.statcounter.com/os-market-share/desktop/worldwide/#monthly-202306-202306-bar) de sistmas operativos, por lo que ciertas aplicaciones y juegos estan pensados para windows 
- soporte de [HDR](https://support.microsoft.com/en-us/windows/hdr-settings-in-windows-2d767185-38ec-7fdc-6f97-bbc6c5ef24e6)
---

# **Desventajas de windows**

---

## Desarrollador
- [java updater](https://www.java.com/en/download/help/java_update.html) esta siempre activo en segundo plano
- ejecuta programas de manera lenta (a tirones) aunque sea pwsh
- [.NET](https://michaelscodingspot.com/dotnet-dll-hell/) y [dll](https://www.partech.nl/en/publications/2022/03/what-is-dll-hell-problem-and-how-to-solve-it) [hell](https://www.baeldung.com/cs/dll-hell-problem)
- Hyper-V y Windows hypervisor platform solo disponibles para [Windows Pro](https://www.microsoft.com/en-us/windows/compare-windows-10-home-vs-pro)
- Virtual Machine Platform, Hyper-V, Windows hypervisor platform y WSL2 interfieren con aplicaciones: [dell alienware control](https://www.dell.com/community/Alienware-Desktops/AWCC-OC-Controls-incompatible-with-Virtual-Machine-Platform/m-p/8239494#M60811), [throttle stop](https://www.techpowerup.com/forums/threads/throttlestop-dead-on-windows-11.284102/), etc.
- los hosts en windows son [read-only](https://superuser.com/questions/958991/windows-10-cant-edit-hosts-file) y modificarlo puede alertar al [antivirus](https://support.microsoft.com/en-au/topic/hosts-file-is-detected-as-malware-in-windows-defender-4320fa8b-0d54-1129-db85-61f095144521)
- para correr un [hello world!](https://stackoverflow.com/questions/55603111/unable-to-compile-rust-hello-world-on-windows-linker-link-exe-not-found) de rust ocupas que descargar visual studio community junto con 1gb para los c++ build tools y el Windows SDK 
- visual studio community usa como [10gb](https://developercommunity.visualstudio.com/t/visual-studio-uses-too-disk-much-space/145475) o [más](https://developercommunity.visualstudio.com/t/hard-disk-space-loss/585904)
- problemas con librerias, aveces tienes que compilarlas manualmente como [pycripto](https://old.reddit.com/r/webdev/comments/132eql/owhy_many_people_dislike_windows_as_an_development/) o en mi caso librespot de rust 
- Problemas de velocidad con [I/O y ntfs](https://github.com/Microsoft/WSL/issues/873)

---

## Uso general
- las apps por defecto se actualizan individualmente ya sea abriendo la aplicación o teniendo que descargar la nueva version de la pagina del creador

- para usar winget ocupas una cuenta microsoft para descargar [App-Installer](https://apps.microsoft.com/store/detail/appinstaller/9NBLGGH4NNS1?hl=de-at&gl=at&rtc=1) de la microsoft store y para usarlo ocupas constantemente aceptar los [UAC](https://learn.microsoft.com/en-us/windows/package-manager/winget/) prompts, aparte de acepatar la [CLA](https://opensource.microsoft.com/cla/) 

- no puedes nombrar archivos con ciertos [nombres](https://yewtu.be/watch?v=bC6tngl0PTI)
- windows pro cuesta [$6399](https://www.microsoft.com/es-mx/d/windows-11-pro/dg7gmgf0d8h4) pesos MXN
- windows 11 [requiere](https://learn.microsoft.com/en-us/windows/whats-new/windows-11-requirements) a tener una cuenta microsoft y usarla en tu sistema
- el sistema operativo se expande hasta más de [40gb](https://superuser.com/questions/1467359/windows-takes-up-40gb-of-disk-space)
- el buscador de windows es [ineficiente](https://computerinfobits.com/why-is-windows-10-search-so-bad/)
- prefetch y superfetch (SysMain), suelen tener el disco duro al [100%](https://yewtu.be/watch?v=MmH4tjH2yMc) de uso 

---

- suele haber más [virus](https://www.howtogeek.com/141944/htg-explains-why-windows-has-the-most-viruses/) que macOS o linux 
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
- pocas opciones open source de customizacion y algunas opciones privadas cuestan [wallpaperengine](https://store.steampowered.com/app/431960/Wallpaper_Engine/), [taskbarX](https://apps.microsoft.com/store/detail/taskbarx/9PCMZ6BXK8GH?hl=en-us&gl=us), [start11](https://www.stardock.com/products/start11/), etc.

---

## hardware
- Device encryption ocupa hardware [moderno](https://www.microsoft.com/en-us/windows/compare-windows-10-home-vs-pro) ([InstantGo](https://blogs.windows.com/windowsexperience/2014/06/19/instantgo-a-better-way-to-sleep/#RXGeiruxOD7f3V0q.97)/[AOAC](https://www.microsoft.com/en-us/store/b/alwaysconnectedfaq)/[HSTI-compliant](https://learn.microsoft.com/en-us/windows-hardware/test/hlk/testref/hardware-security-testability-specification)), basicamente de 2014 en adelante.
- los [requisitos](https://www.microsoft.com/en-us/windows/windows-11-specifications) de Windows 11, procesador de 64 bits, UEFI, TPM v2.0 y una grafica compatible con DirectX12.
- los discos duros con ntfs tienen que [defragmentarse](https://learn.microsoft.com/en-us/previous-versions/cc767961(v=technet.10))
- los drivers oficiales de nvidia tienen [telemetria](https://www.geeks3d.com/20161107/nvidia-telemetry-in-geforce-drivers/)
- no suele haber drivers opensource


## juegos
- descargas [muchas versiones](https://www.howtogeek.com/256245/why-are-there-so-many-microsoft-visual-c-redistributables-installed-on-my-pc/) de microsoft visual c++ redistributable por juego
- los juegos de la microsoft store (xbox app) suelen correr [peor](https://old.reddit.com/r/techsupport/comments/v4nhaf/so_ive_been_wondering_if_its_just_me_or_windows/) o dar [input lag](https://www.reddit.com/r/roblox/comments/oahvsf/roblox_player_vs_microsoft_store_app_input_lag/)
- no puedes acceder a las [carpetas](https://www.makeuseof.com/windows-access-windowsapps-folder/) de juegos de la microsoft store (xbox app) aun siendo administrador


---

## privacidad
- botones de anti privacidad activados por [defecto](https://learn.microsoft.com/es-es/intune-education/media/rs5_choose_settings.png)
- windows [phone home](https://yewtu.be/watch?v=IT4vDfA_4NI).
- windows hace backdoors para [NSA](http://techrights.org/wiki/index.php/Microsoft_and_the_NSA) y esta involucrado con [PRISM](https://en.wikipedia.org/wiki/PRISM)
- datos de diagnosticos [obligatorios](https://learn.microsoft.com/en-us/windows/privacy/required-windows-diagnostic-data-events-and-fields-2004)
- [edge](https://learn.microsoft.com/en-us/microsoft-edge/privacy-whitepaper/) y [office](https://learn.microsoft.com/en-us/deployoffice/compat/data-that-the-telemetry-agent-collects-in-office) envian telemetria
- [Delivery Optimization](https://learn.microsoft.com/en-us/windows/deployment/do/waas-delivery-optimization) esta activado por [defecto](https://www.dell.com/support/kbdoc/es-mx/000125580/information-on-the-windows-update-delivery-optimization-feature-within-windows-10?lang=en)
- la [declaración de privacidad](https://privacy.microsoft.com/en-us/privacystatement)

---

# más referencias de las desventajas de windows
- [GNU: Microsoft's Software is Malware](https://www.gnu.org/proprietary/malware-microsoft.en.html)
- [reddit: why many people dislike windows as an development environment?](https://old.reddit.com/r/webdev/comments/132eql/why_many_people_dislike_windows_as_an_development/)
- [reddit: what is your worst experience with ms windows?](https://old.reddit.com/r/linuxmasterrace/comments/u19uee/what_is_your_worst_experience_with_ms_windows/)
- [reddit: why so much hate to windows?](https://old.reddit.com/r/linuxmasterrace/comments/qi370x/why_so_much_hate_to_windows/)
- [Wikipedia: Criticism of Microsoft](https://en.wikipedia.org/wiki/Criticism_of_Microsoft)
- [installgentoo wiki: Windows](https://wiki.installgentoo.com/wiki/Windows)
- [installgentoo wiki: Windows 10](https://wiki.installgentoo.com/wiki/Windows_10)
- [itvision blog: why windows 10 sucks](https://itvision.altervista.org/why-windows-10-sucks.html)
- [itvision blog: why windows 11 sucks](https://itvision.altervista.org/why-windows-11-sucks.html)
- [Jody Bruchon Tech: Windows 11 Must Be Stopped - A Veteran PC Repair Shop Owner's Dire Warning](https://yewtu.be/watch?v=LcafzHL8iBQ)

---

# Recomendaciones si tienes que usar windows
- usa windows 10 sin iniciar sesion en una cuenta de microsoft
- descarga apps de la ms store con https://store.rg-adguard.net/
- usa windows  en una vm  con NAT activado
- instala drivers de nvidia sin telemetria con [nvclean](https://www.techpowerup.com/download/techpowerup-nvcleanstall/) 
- si es para jugar, preinstala todos los Visual C++ desde [techpowerup](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)
- usa [Chris Titus Tech's Windows Utility](https://github.com/ChrisTitusTech/winutil) para desactivar facilemente telemetria y otras funcionalidades como activar UTC para usar windows en dual-boot
- bloquea paginas en el archivo de [hosts](https://gist.github.com/VirtuBox/f09968a2d27bc00ba58b3617c61dc54e)
- prueba que el software descargado de internet no tenga virus con [virustotal](https://www.virustotal.com/gui/)
-  usa aplicaciones con posibles virus en [sandboxie](https://sandboxie-plus.com/)
- [autoruns](https://learn.microsoft.com/en-us/sysinternals/downloads/autoruns) para desactivar apps/servicios al inicio del sistema 
- usa [scoop](https://scoop.sh/) como package manager

---

# **linux distributions**

---

una distribucion de linux es:
las distribuciones se pueden diferenciar por tres partes principales:
el sistema de arranque (init system (PID 1)), gestor de paquetes (package manager) y su filosofia (uso,caracteristicas,orientacion,etc.)

categorias de distribuciones:

independiente: la ventaja de esta es tener otras opciones
deribados: los deribados tienen compatibilidad con quien se deribaron

tipos de distribuciones deribadas:

 flavour: otros escritorios o temas oficiales de la distribucion, por ejemplo para ubuntu hay flavours como: edubuntu,kubuntu,lubuntu, etc.
 remix/respin: agregando un objetivo especifico 
 fork
 clone/repackage: copian el codigo y tienen otra infrestructura para la distribucion, por ejemplo para RHEL hay repackages como Rocky linux, Oracle Linux, etc.

rolling release
bleeding edge

---

<style scoped>table {font-size: 23px;}</style>

## independentes 

| distribucion | init           | pkg manager | filosofia    |
|--------------|----------------|-------------|--------------|
| [alpine](https://alpinelinux.org/)       | openrc         | apk         | no gnu       |
| [arch](https://archlinux.org/)         | systemd        | pacman      | bleeding edge|
| [debian](https://www.debian.org/)       | systemd        | apt         | community    |
| [slackware](http://www.slackware.com/)    | sysV           | slackpkg    | kiss         |
| [SUSE](https://www.suse.com/products/server/) LE S/D      | systemd        | zipper      | enterprise   |
| [gentoo](https://www.gentoo.org/)       | OpenRC/systemd | portage     | compile      |
| [void](https://voidlinux.org/)         | runit          | xbps        | BSD-feel     |
| [nixos](https://nixos.org/)        | systemd        | nix         | portability  |
| [RHEL](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux)         | systemd        | yum         | enterprise   |

---

<style scoped>table {font-size: 23px;}</style>

## deribadas

| distribucion | init             | basado en   | filosofia 
|--------------|------------------|-------------|-----------
| [artix](https://artixlinux.org/)        | OpenRC/runit/etc. | arch        | no systemd
| [devuan](https://www.devuan.org/)       | sysV/OpenRC/etc.           | debian      | no systemd
| [Ubuntu](https://ubuntu.com/)       | systemd          | debian      | enterprise
| [Uaabuntu](https://uaabuntu.uaa.mx/)     | systemd          | ubuntu      | educacion
| [openSUSE](https://opensuse.org/)     | systemd          | SUSE        | community
| [parabola](https://www.parabola.nu/)     | systemd/OpenRC/etc. | arch        | Linux-libre
| [Fedora](https://fedoraproject.org/)       | systemd          | RHEL        | comunitty

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

<style scoped>{font-size: 21px;}</style>

 - Michael Tunnell. (2023). *Explaining Linux Family Trees: Why Are There So Many Linux Distros?* [Video]. https://yewtu.be/watch?v=kF8CRt05s6A
- The Linux Information Project. (2005). *Flavors of UNIX Definition*. http://www.linfo.org/flavors.html






- Adekotujo, A., Odumabo, A., Adedokun, A., & Aiyeniko, O. (2020). *A Comparative Study of Operating Systems: Case of Windows, UNIX, Linux, Mac, Android and iOS*. https://www.researchgate.net/profile/Adedoyin-Odumabo/publication/343013056_A_Comparative_Study_of_Operating_Systems_Case_of_Windows_UNIX_Linux_Mac_Android_and_iOS/links/61f2b50a9a753545e2fe8300/A-Comparative-Study-of-Operating-Systems-Case-of-Windows-UNIX-Linux-Mac-Android-and-iOS.pdf
- The Open Group. (2008). *The Single UNIX Specification, Version 4*. https://unix.org/version4/overview.html
- IEEE. (2017). *IEEE Std 1003.1™-2017*. https://pubs.opengroup.org/onlinepubs/9699919799/

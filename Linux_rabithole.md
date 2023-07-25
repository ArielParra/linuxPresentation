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
1. ¿Qué es linux?
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

# 1.3 temas relacionadas


# FOSS
Free and open source software

- creative commons: uso libre pero con atribucion obligatoria
![CC BY](https://licensebuttons.net/l/by/3.0/88x31.png), ![CC BY-SA](https://licensebuttons.net/l/by-sa/3.0/88x31.png), ![CC BY-ND](https://licensebuttons.net/l/by-nd/3.0/88x31.png), ![CC BY-NC](https://licensebuttons.net/l/by-nc/3.0/88x31.png), ![CC BY-NC-SA](https://licensebuttons.net/l/by-nc-sa/3.0/88x31.png) y ![CC BY-NC-ND](https://licensebuttons.net/l/by-nc-nd/3.0/88x31.png)
- licencias más comunes:
    - Apache: incluya la nota de copyright  
    - BSD: incluya la nota de copyright 
    - GPL: codigo fuente disponible y trabajos deribados con la misma licencia 
    - MIT: incluya la nota de copyright  
herramienta para elegir una [licencia](https://choosealicense.com/) adecuada
- Free/libre: la filosofia free tiene relacion con richard stallman y su proyecto GNU, esta se basa en software que respeta la libertad del usuario, libertad de distrubucion, libertad de uso, libertad de estudio, etc. llendo en contra del software privado de codigo cerrado, los binary blobs, las licencias y EULAs no permisivas, los  y el DRM.

---

# UNIX

UNIX es un sistema operativo creado a principios de los 70s en AT&T por Dennis Ritchie (creador del lenguaje C) y Ken Thompson (creador de B predecesor del lenguaje C) 
- POSIX: "Portable Operating System Interface", son una serie de standares de uso impuestos por el IEEE (Institute of Electrical and Electronics Engineers) que incluye el I/O, la terminal, comandos y redes.
- Single UNIX Specification: es un estandard para sistemas operativos para usar el tredemark de UNIX, con interfaces para el lenguaje C, el shell y comandos especificos como por ejemplo "echo".
- UNIX filosofy (Doug McIlroy):
Escribe programas que hagan una cosa muy bien, escribe programas que trabajen juntos (input de uno es el output de otro). Escribe programas que manejen streams (serie de bytes para I/O), porque son  una interfaz universal.
- todo son archivos, los dispositivos, teclados, discos duros, etc. estos son manejados con streams
- Lenguaje C es superior
- los sistemas BSD son más unix que linux

---

# bsd

"Berkeley Software Distribution" es un sistema operativo creado en la universidad de Berkeley en California, de codigo abierto y originalmente extension de AT&T’s Research UNIX, a diferencia de linux este tiene la BSD C library, aunque pueden compartir ciertas utilidades de GNU

los dos forks más importantes son:
- freeBSD: es un proyecto ["grande"](https://svnweb.freebsd.org/base/stable/12/) con muchos sistemas operativos forkeados apartir de el, como FreeNAS, pfsense, etc.
- OpenBSD: es un proyecto relativamente mas ["chico"](https://cvsweb.openbsd.org/src/) que freebsd, es [inovador](https://www.openbsd.org/innovations.html
) y crean nuevas herramientas usadas en toda la comunidad unix, mientras que es de los sistemas más seguros

estos pueden tener ciertas [ventajas y desventajas](https://serverfault.com/questions/5267/what-is-good-about-the-bsds/5352#5352) a linux


---

# minimalismo
el minimalismo en cuestion de linux, se trata de usar y escribir programas simples siguiendo principios de UNIX y KISS (Keep it simple, stupid!),  dos ideas deribadas del minimalismo son:
- gnuless: algunos programas de GNU pueden no ser los más eficientes o minimalistas, un video acerca del tema: [Luke Smith: GNU is bloated!](https://yewtu.be/watch?v=nTCHapo8QFM)
- init freedom: systemd es el init system más usado, pero este no sigue la filosofia de unix ya que systemd no solo es el init ya que tiene muchas otras funcinoes y herramientas, por lo que usar alternativas es recomendado

---

# Privacidad 

te recominedo esta [guia](https://www.privacyguides.org/en/) de privacidad
[duckduckgo](https://seonorth.ca/news/why-duckduckgo-is-bad/) no es bueno
[proton](https://techcrunch.com/2021/09/06/protonmail-logged-ip-address-of-french-activist-after-order-by-swiss-authorities/) no es confiable
las VPN no te dan [privacidad](https://gist.github.com/joepie91/5a9909939e6ce7d09e29)
tor y sus [mitos](https://www.whonix.org/wiki/Tor_Myths_and_Misconceptions)

# Seguridad

te recomiendo esta [guia](https://wiki.archlinux.org/title/security) de seguridad
[linux-hardened](https://github.com/anthraxx/linux-hardened) kernel
[selinux](https://selinuxproject.org/page/Main_Page) o [AppArmor](https://apparmor.net/) para el control de acceso
no uses [kali linux](https://www.kali.org/docs/introduction/should-i-use-kali-linux/)
usa OpenBSD, ya que es el sistema unix más [seguro](https://www.openbsd.org/security.html)

---

# customizacion (ricing)

solo mira [r/unixporn](https://reddit.com/r/unixporn/)
[dotfiles](https://wiki.archlinux.org/title/Dotfiles) son los archivos que van en la carpeta de usuario y tienen las configuraciones de los programas que se van a costumizar
tambien puedes usar una distrubucion que ya venga riceada como [archcraft](https://archcraft.io/gallery.html)

---

# 1.4 ventajas de linux 
- es gratuito y opensource
- superioridad en cuestion de audio con [pipewire](https://pipewire.org/)
- puede arrancar [rapidamente](https://www.forbes.com/sites/jasonevangelho/2019/06/19/infographics-linux-mint-challenges-windows-10-in-small-business-speed-tests-laptop/#7a560d2369bb) el sistema y las aplicaciones
- tiempos menores de [compilacion](https://medium.com/aedm/windows-wsl-and-linux-a-build-time-benchmark-for-java-rust-go-and-node-43188a9c77d6)
- mejores resultados en [geekbench](https://yewtu.be/watch?v=7BreeFlhP78)
- usa menos memoria [RAM](https://yewtu.be/watch?v=L3d9okxKcjM)
- es [portable](https://www.oreilly.com/library/view/linux-kernel-development/0672327201/ch19.html)
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
- [The Linux Foundation: Why are Linux Jobs so In Demand?](https://training.linuxfoundation.org/blog/why-are-linux-jobs-so-in-demand/)
- [The Linux Experiment: Windows, macOS & Linux PRIVACY compared: why do they need ALL THIS DATA?!](https://yewtu.be/watch?v=MMc5zgALLiY)

---
# desventajas de linux

- tienes que aprender temas nuevos, aprender a buscar soluciones y leer.
- no puedes correr ciertos juegos: [rainbow six](https://www.protondb.com/app/359550), [roblox](https://news.itsfoss.com/roblox-linux-end/), [etc.](https://www.protondb.com/explore?sort=fixWanted)
- no puedes correr ciertas aplicaciones: [Adobe Photoshop](https://appdb.winehq.org/objectManager.php?sClass=application&iId=17), [MS Office](https://appdb.winehq.org/objectManager.php?sClass=application&iId=31), [etc](https://appdb.winehq.org/).
- sin soporte completo para [HDR](https://wiki.archlinux.org/title/HDR_monitor_support) 
- problemas con [variable refresh rate](https://wiki.archlinux.org/title/Variable_refresh_rate)
- problemas con [fractional scaling](https://wiki.archlinux.org/title/HiDPI)
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
- puedes compartir pantalla con sonido en [discord](https://support.discord.com/hc/en-us/articles/1500006741102-macOS-Screen-Share-with-Audio-Update-FAQ) y [MS Teams](https://answers.microsoft.com/en-us/msteams/forum/all/sharing-system-sound-in-teams-for-linux/f1c70d83-e9bd-41b4-abde-d78fae764d5c)
- buen rendimiento en juegos con [D3DMetal](https://developer.apple.com/metal/) y  [game porting toolkit](https://old.reddit.com/r/macgaming/comments/1446hj6/all_working_games_list_game_porting_toolkit/)

---

# desventajas MacOS

- Appple ID es un requisito para instalar MacOS
- no puede correr ciertos [juegos](https://www.protondb.com/explore?sort=fixWanted)
- quitaron el soporte de [32-bits](https://support.apple.com/en-us/HT208436) y con eso muchas  [apps](https://gist.github.com/stevemoser/a4388df17633beae5bc3fb07d38373e2)
- hardware [oficial](https://everymac.com/systems/apple/index-apple-specs-applespec.html) y [no oficial](https://hackintosh.com/#hackintosh_compatible) limitados
- las computadoras Mac son [costosas](https://everymac.com/global-mac-prices/mac-prices-mexico-mx.html)
- la existencia de [OCSP](https://blog.jacopo.io/en/post/apple-ocsp/)
- multiples problemas de [privacidad](https://sneak.berlin/20201112/your-computer-isnt-yours/)
- los [contratos de licencia de software](https://www.apple.com/legal/sla/)
- posibles conexiones con NSA e implicacion con [PRISM](https://www.washingtonpost.com/investigations/us-intelligence-mining-data-from-nine-us-internet-companies-in-broad-secret-program/013/06/06/3a0c0da8-cebf-11e2-8845-d970ccb04497_story.html)
- no suele haber drivers opensource
- la capa de compatibilidad con windows wine puede correr [malware](https://wiki.winehq.org/FAQ#Is_Wine_malware-compatible.3F)
- no tiene controles de volumen por [aplicacion](https://apple.stackexchange.com/questions/381397/is-it-possible-to-set-an-individual-sound-volume-for-each-program-on-a-mac)

---

# Recomendaciones si tienes que usar MacOS
- no uses una cuenta de Apple ID con tus datos personales
- usa macOS en una vm con NAT activado
- lee esta [guia](https://github.com/drduh/macOS-Security-and-Privacy-Guide) de privacidad en MacOS
- usa [alacritty](https://alacritty.org/) como emualdor terminal
- usa [brew](https://brew.sh/) como package manager

---

# ventajas de windows
- compatibilidad perfecta con [directX](https://www.microsoft.com/en-us/download/details.aspx?id=35)
- [compatibilidad](https://support.microsoft.com/en-us/windows/make-older-apps-or-programs-compatible-with-windows-783d6dd7-b439-bdb0-0490-54eea0f45938) con aplicaciones antiguas de windows
- las empresas les importa la distribucion del [mercado](https://gs.statcounter.com/os-market-share/desktop/worldwide/#monthly-202306-202306-bar) de sistmas operativos, por lo que ciertas aplicaciones y juegos estan pensados para windows 
- soporte de [HDR](https://support.microsoft.com/en-us/windows/hdr-settings-in-windows-2d767185-38ec-7fdc-6f97-bbc6c5ef24e6)
- Windows Subsystem for Linux [(WSL)](https://learn.microsoft.com/en-us/windows/wsl/about)  y Windows Subsystem for Android [(WSA)](https://learn.microsoft.com/en-us/windows/android/wsa/)

---

# Desventajas de windows

---

## Desarrollador
- [java updater](https://www.java.com/en/download/help/java_update.html) esta siempre activo en segundo plano
- ejecuta programas de manera lenta (a tirones) aunque sea pwsh
- [.NET](https://michaelscodingspot.com/dotnet-dll-hell/) y [dll](https://www.partech.nl/en/publications/2022/03/what-is-dll-hell-problem-and-how-to-solve-it) [hell](https://www.baeldung.com/cs/dll-hell-problem)
- Hyper-V y Windows hypervisor platform solo disponibles para [Windows Pro](https://www.microsoft.com/en-us/windows/compare-windows-10-home-vs-pro)
- Virtual Machine Platform, Hyper-V, Windows hypervisor platform y WSL2 interfieren con aplicaciones: [dell alienware control](https://www.dell.com/community/Alienware-Desktops/AWCC-OC-Controls-incompatible-with-Virtual-Machine-Platform/m-p/8239494#M60811), [throttle stop](https://www.techpowerup.com/forums/threads/throttlestop-dead-on-windows-11.284102/), etc.
- los hosts en windows son [read-only](https://superuser.com/questions/958991/windows-10-cant-edit-hosts-file) y modificarlo puede alertar al [antivirus](https://support.microsoft.com/en-au/topic/hosts-file-is-detected-as-malware-in-windows-defender-4320fa8b-0d54-1129-db85-61f095144521)
- para correr un ["hello world!"](https://stackoverflow.com/questions/55603111/unable-to-compile-rust-hello-world-on-windows-linker-link-exe-not-found) de rust ocupas que descargar visual studio community junto con 1gb para los c++ build tools y el Windows SDK 
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
- los antivirus pueden bloquear aplicaciones/servicios en el [firewall](https://www.mcafee.com/support/?locale=en-US&articleId=TS102946&page=shell&shell=article-view) 
- Windows Antimalware Service puede usar [100%](https://answers.microsoft.com/en-us/windows/forum/all/high-cpu-usage-by-antimalware-service-executable/4f6f635a-b3ad-444c-8cd0-68fb1e9f4bfa) del cpu
- Problemas en pantallas con [high dpi](https://support.microsoft.com/en-gb/topic/windows-scaling-issues-for-high-dpi-devices-508483cd-7c59-0d08-12b0-960b99aa347d) dando lugar a [apps borrosas](https://support.microsoft.com/en-us/windows/fix-apps-that-appear-blurry-in-windows-10-e9fe34ab-e7e7-bc6f-6695-cb169b51de0f)
- la solucion a la mayoria de errores es [reistalar](https://answers.microsoft.com/en-us/windows/forum/all/windows-update-system-restore-and-repair-failed/aaf28405-55c0-4ee2-b4b4-f13571680b32) el sistema operativo
- las [apps](https://www.pcmag.com/how-to/stop-windows-10-apps-from-launching-at-startup) se ejecutan al inicio o crean servicios que se ejecutan al inicio
- fondos de pantalla en slidehow puede no [funcionar](https://answers.microsoft.com/en-us/windows/forum/all/background-slideshow-stops-working/acfcabe4-56fb-436a-afc6-42bdd877ca29)
- pocas opciones open source de [customizacion](https://github.com/Awesome-Windows/Awesome#customization) y algunas opciones privadas cuestan [wallpaperengine](https://store.steampowered.com/app/431960/Wallpaper_Engine/), [taskbarX](https://apps.microsoft.com/store/detail/taskbarx/9PCMZ6BXK8GH?hl=en-us&gl=us), [start11](https://www.stardock.com/products/start11/), etc.

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
- opciones anti privacidad activados por [defecto](https://learn.microsoft.com/es-es/intune-education/media/rs5_choose_settings.png)
- windows [phone home](https://yewtu.be/watch?v=IT4vDfA_4NI).
- windows esta implicacdo con la [NSA](http://techrights.org/wiki/index.php/Microsoft_and_the_NSA) y [PRISM](https://en.wikipedia.org/wiki/PRISM)
- datos de diagnosticos [obligatorios](https://learn.microsoft.com/en-us/windows/privacy/required-windows-diagnostic-data-events-and-fields-2004)
- [edge](https://learn.microsoft.com/en-us/microsoft-edge/privacy-whitepaper/) y [office](https://learn.microsoft.com/en-us/deployoffice/compat/data-that-the-telemetry-agent-collects-in-office) envian telemetria
- [Delivery Optimization](https://learn.microsoft.com/en-us/windows/deployment/do/waas-delivery-optimization) esta activado por [defecto](https://www.dell.com/support/kbdoc/es-mx/000125580/information-on-the-windows-update-delivery-optimization-feature-within-windows-10?lang=en)

---

# más referencias de las desventajas de windows
- [GNU: Microsoft's Software is Malware](https://www.gnu.org/proprietary/malware-microsoft.en.html)
- [Jody Bruchon Tech: Windows 11 Must Be Stopped - A Veteran PC Repair Shop Owner's Dire Warning](https://yewtu.be/watch?v=LcafzHL8iBQ)
- [reddit: why many people dislike windows as an development environment?](https://old.reddit.com/r/webdev/comments/132eql/why_many_people_dislike_windows_as_an_development/)
- [reddit: what is your worst experience with ms windows?](https://old.reddit.com/r/linuxmasterrace/comments/u19uee/what_is_your_worst_experience_with_ms_windows/)
- [reddit: why so much hate to windows?](https://old.reddit.com/r/linuxmasterrace/comments/qi370x/why_so_much_hate_to_windows/)
- [Wikipedia: Criticism of Microsoft](https://en.wikipedia.org/wiki/Criticism_of_Microsoft)
- [installgentoo wiki: Windows](https://wiki.installgentoo.com/wiki/Windows)
- [installgentoo wiki: Windows 10](https://wiki.installgentoo.com/wiki/Windows_10)
- [itvision blog: why windows 10 sucks](https://itvision.altervista.org/why-windows-10-sucks.html)
- [itvision blog: why windows 11 sucks](https://itvision.altervista.org/why-windows-11-sucks.html)

---

# Recomendaciones si tienes que usar windows
- usa windows 10 sin iniciar sesion en una cuenta de microsoft
- descarga apps de la ms store con https://store.rg-adguard.net/
- usa windows  en una vm  con NAT activado
- si usas windows en una vm usa [WinApps](https://github.com/Fmstrat/winapps)
- si usas una grafica nvidia, instala drivers sin telemetria con [nvcleanstall](https://www.techpowerup.com/download/techpowerup-nvcleanstall/) 
- si es para jugar, preinstala todos los Visual C++ desde [techpowerup](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)
- usa [Chris Titus Tech's Windows Utility](https://github.com/ChrisTitusTech/winutil) para desactivar facilemente telemetria o tambien para activar UTC si se usa windows en dual-boot
- bloquea las direcciones a donde se envian telemetrias en el archivo de [hosts](https://gist.github.com/VirtuBox/f09968a2d27bc00ba58b3617c61dc54e)
- prueba que el software descargado de internet no tenga virus con [virustotal](https://www.virustotal.com/gui/)
-  usa aplicaciones con posibles virus en [sandboxie plus](https://sandboxie-plus.com/)
- [autoruns](https://learn.microsoft.com/en-us/sysinternals/downloads/autoruns) para desactivar apps/servicios al inicio del sistema 
- usa [alacritty](https://alacritty.org/) como emualdor terminal y usa [scoop](https://scoop.sh/) como package manager

---

# **Distribuciones de linux**

---

# ¿Qué es?
una distribucion (distro) de linux es un sistema operativo completo con muchos componentes opensource.

---

los componentes y caracteristicas que construyen a una distribucion de linux son: 
- filosofia: KISS, free/libre, utilitarism, bsd feel, unix feel,  etc.
- licencia: BSD, gnu GPL v2, gnu GPL v3, MIT, etc.
- uso especifico:
    - juegos: steamOS, ChimeraOS, popOS, Fedora Games spin, etc.
    - media: Ubuntu Studio, Fedora Design Suite, etc.
    - escolar: uaabuntu, edubuntu, Zorin OS Education, etc.
    - privacidad/seguridad: whonix y/o qubes, tails, etc. 
- Release model : fix, rolling release, lts, bleeding edge
- Boot Loader: GRUB, Syslinux, LILO, systemd-boot, etc.
- tipo de kernel: Stable (vanilla), zen, libre, LTS, Realtime, etc.
- init system / daemon manager: runit, OpenRC, systemd, SysVinit, s6, dinit, etc.
- systema de archivos (File system): ext2/3/4, Btrfs, XFS, ZFS, etc. 
- jerarquia de archivos: Linux File Hierarchy Structure o modificacion de este. 
- libreria de c: glibc, musl, ulibc, etc.
- utilidades basicas: gnu core utils + util-linux, busybox, etc.

---

- interfaz de shell: bash, zsh, fish, dash, ash, etc.
- servidor grafico: Xorg (X11) / protocolo grafico: Wayland 
- tecnologia de audio: pulseaudio, Jack, Alsa, pipewire.
- login manager: ssdm (KDE)
- window manager: dwm, sway, i3, xmonad, etc.    
- Desktop environment: Gnome, Plasma, xfce4, etc. 
- Graphics Toolkits: GTK+ / Qt
- gestor de paquetes (package manager): apt, DNF, pacman, portage, yay, etc.
- formato de paquetes: deb, RPM, .pkg.tar.zst, source code, install scripts, etc.

---

- repositorio de paquetes de la distribucion
- aplicaciones incluidas: 
    - terminal (CLI/TUI):
        - editor de textos: nano, vim, neovim, emacs, etc.
    - graficas (GUI):
        - navegador: firefox, chromium, etc.
        - Office Suite: libreoffice, onlyoffice, Calligra etc.
        - emulador de terminal: konsole, gnome-terminal, alacritty, kitty, st, etc. 
        - editor de textos: vscodium, gvim, etc.
        - explorador de archivos: nautilus (gnome), dolphin (KDE)
        - visualizador de imagenes: feh, gwenviwer, etc.

---

hay cuatro partes que definen y diferencian a una distribucion de linux son:
el sistema de arranque (init system [PID 1]), gestor de paquetes (package manager), libreria de c y las core utils, esto se debe a que todo lo demas lo puedes modificar a tu gusto con facilidad.

categorias de distribuciones:
- independiente: la ventaja de esta es tener otras opciones
 deribados: los deribados tienen compatibilidad con quien se deribaron
 sinergia de distribuciones: debian <-> ubuntu, SUSE <-> openSUSE,
 RHEL <-> fedora.
 
- tipos de distribuciones deribadas:
    - flavour: con otros escritorios,temas, y/o aplicaiones reconocidos por la distribucion, por ejemplo para ubuntu hay flavours como: edubuntu,kubuntu,lubuntu, etc.
    - remix/respin: modificacion ofreciendo algo nuevo, pero sin ser reconocidos por la distribución.
    - fork: hacen cambios grandes, cambiando el uso, filosofia, etc.
    - clone/repackage: copian el codigo y tienen otra infrestructura para la distribucion, por ejemplo para RHEL hay repackages como Rocky linux, Oracle Linux, etc.

[Linea de tiempo](https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg)

---

<style scoped>table {font-size: 25px; text-align: center }</style>

## independentes 

| Logo                           | distribucion                                                                   | init           | pkg manager | libreria c | core utils  |  
|--------------------------------|--------------------------------------------------------------------------------|----------------|-------------|------------|-------------|
| ![h:50](logos/alpine.png)      | [alpine](https://alpinelinux.org/)                                             | openrc         | apk         | musl       | busybox     |
| ![h:50px](logos/arch.png)      | [arch](https://archlinux.org/)                                                 | systemd        | pacman      | glibc      | gnu         |
| ![h:50px](logos/debian.png)    | [debian](https://www.debian.org/)                                              | systemd        | apt (dpkg)  | glibc      | gnu         |
| ![h:50px](logos/slackware.png) | [slackware](http://www.slackware.com/)                                         | sysVinit           | slackpkg    | glibc      | gnu         |
| ![h:50px](logos/gentoo.png)    | [gentoo](https://www.gentoo.org/)                                              | OpenRC/systemd | portage     | glibc/musl | gnu         |
| ![h:50px](logos/void.png)      | [void](https://voidlinux.org/)                                                 | runit          | xbps        | glibc/musl | gnu         |

---

<style scoped>table {font-size: 25px; text-align: center }</style>


| Logo                        | distribucion                                                                   | init         | pkg manager | libreria c | core utils  |  
|-----------------------------|--------------------------------------------------------------------------------|--------------|-------------|------------|-------------|
| ![h:50px](logos/nixos.png)  | [nixos](https://nixos.org/)                                                    | systemd      | nix         | glibc      | gnu         |
| ![h:50px](logos/RHEL.png)   | [RHEL](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux)| systemd      | DNF (yum)   | glibc      | gnu         |
| ![h:70px](logos/SUSE.png)   | [SUSE LE S/D](https://www.suse.com/products/server/)                           | systemd      | Zypper      | glibc      | gnu         | 
| ![h:50px](logos/LFS.png)    | [LFS](https://www.linuxfromscratch.org/lfs/)                                   | systemd/sysV | -           | glibc      | gnu         | 
| ![h:50px](logos/kiss.png)   | [kiss](https://kisslinux.org/)                                                 | runit        | kiss        | musl       | busybox     | 
| ![h:50px](logos/chimera.png)| [chimera-linux](https://chimera-linux.org/)                                    | Dinit        | apk         | musl       | BSD-derived | 

---

<style scoped>table {font-size: 25px; text-align: center }</style>

## deribadas

| Logo                          | distribucion                          | init               | basado en   | libreria c | core utils  |  
|-------------------------------|---------------------------------------|--------------------|-------------|------------|-------------|
| ![h:50px](logos/artix.png)    |[artix](https://artixlinux.org/)       | OpenRC/runit/etc.  | arch        | glibc      | gnu         |
| ![h:50px](logos/devuan.png)   |[devuan](https://www.devuan.org/)      | sysV/OpenRC/etc.   | debian      | glibc      | gnu         |
| ![h:50px](logos/ubuntu.png)   |[Ubuntu](https://ubuntu.com/)          | systemd            | debian      | glibc      | gnu         |
| ![h:50px](logos/uaabuntu.png) |[Uaabuntu](https://uaabuntu.uaa.mx/)   | systemd            | ubuntu      | glibc      | gnu         |
| ![h:50px](logos/openSUSE.png) |[openSUSE](https://opensuse.org/)      | systemd            | SUSE        | glibc      | gnu         |

---

<style scoped>table {font-size: 25px; text-align: center }</style>

| Logo                           | distribucion                           | init               | basado en     | libreria c | core utils  |  
|--------------------------------|----------------------------------------|--------------------|---------------|------------|-------------|
| ![h:50px](logos/fedora.png)    |[Fedora](https://fedoraproject.org/)    | systemd            | RHEL          | glibc      | gnu         |
| ![h:50px](logos/endeavour.png) |[endeavour](https://endeavouros.com/)   | systemd            | arch          | glibc      | gnu         |
| ![h:50px](logos/archcraft.png) |[archcraft](https://archcraft.io/)      | systemd            | arch          | glibc      | gnu         |
| ![h:50px](logos/PopOS.png)     |[PopOS](https://pop.system76.com/)      | systemd            | ubuntu/debian | glibc      | gnu         |
| ![h:50px](logos/mint.png)      |[Mint](https://linuxmint.com/)          | systemd            | ubuntu/debian | glibc      | gnu         |
| ![h:50px](logos/elementary.png)|[elementary](https://elementary.io/)    | systemd            | ubuntu/debian | glibc      | gnu         |
| ![h:50px](logos/zorin.png)|[zorin](https://zorin.com/os/)    | systemd            | ubuntu/debian | glibc      | gnu         |

---

<style scoped>table {font-size: 25px; text-align: center }</style>

# Recomendadas por la FSF (linux-libre kernel)
| Logo                          | distribucion                            | init               | basado en     | pkg manager | libreria c | core utils  |  
|-------------------------------|-----------------------------------------|--------------------|---------------|-------------|------------|-------------|
| ![h:50px](logos/parabola.png) | [parabola](https://www.parabola.nu/)    | systemd/OpenRC/etc.| arch          | pacman      | glibc      | gnu         |
| ![h:50px](logos/Hyperbola.png)| [hyperbola](https://www.hyperbola.info/)| OpenRC             | debian/arch   | pacman      | glibc      | gnu         |
| ![h:50px](logos/Guix.png)     | [Guix](https://guix.gnu.org/)           | shepherd           | independiente | Guix        | glibc      | gnu         | 
| ![w:300px](logos/PureOS.png)  | [PureOs](https://pureos.net/)           | systemd            | debian        | apt         | glibc      | gnu         | 
| ![h:50px](logos/trisquel.png) | [trsiquel](https://trisquel.info/)      | systemd            | ubuntu/debian | apt         | glibc      | gnu         | 

---

# que conforma linux
unix filosofy
todos son archivos
sistema jerarquia 
componentes

# linux commands (gnu core utils)

https://wiki.archlinux.org/title/core_utilities 
gnu core utils https://wiki.debian.org/coreutils + util-linux   https://en.wikipedia.org/wiki/Util-linux
busybox https://busybox.net/downloads/BusyBox.html

posix https://en.wikipedia.org/wiki/Category:Unix_SUS2008_utilities

# aplicaciones 

aplicacion y dependencias

portables:
app image, snap, flatpak

aplicaiones recomendadas:
IDE: vscodium
editor de texto: vim
navegador: librewolf + arkenfox user.js o ungoogled-chromium
motor de busqueda: searXNG 
torrents: qbitorrent-enhanced
terminal: alacritty o st
monitor de recursos: btop

# hardware
libreboot/coreboot para desabilitar AMD PSP, intel ME
que es AMD PSP:
que es intel ME:
se puede eliminar completamente en procesadores intel core duo
se puede deshabilitar en una gran parte con: [me_cleaner](https://github.com/system76/coreboot/tree/8c9e6ad9833bfdc522917200e0101c84fe0784c2/util/me_cleaner)
si deshabilitar intel ME en procesadores de la 11 generacion (Tiger-Lake) en adelante, se usa el [triple de energia](https://github.com/system76/firmware-open/blob/master/docs/intel-me.md#tiger-lake-u) en estado de suspencion 

microcode es un blob necesario para sacar el mejor rendimiento al procesador
undervolting es una [vulnerabilidad](https://plundervolt.com/)
fsf 

vendedores de laptops/computadoras con coreboot: 
[starlabs](https://mx.starlabs.systems/)
[tuxedo](https://www.tuxedocomputers.com/index.php)
[system76](https://system76.com/)

hardware y computadoras sin ningun binario o software propietario:
[libreboot list](https://libreboot.org/docs/hardware/)
[h-node](https://h-node.org/hardware/catalogue/en)
[FSF Recommended Complete Systems](https://www.fsf.org/resources/hw/systems)
https://h-node.org/hardware/catalogue/en
[Respects Your Freedom Certification](https://ryf.fsf.org/index.php/products)

---


# distribucion de mercado
# servidores

las distribuciones más usadas en la industria son las empresariales:
RHEL, SLES y las basdas en debian: debian, ubuntu server y proxmox

hardware para servidores:
x64: intel xeon,amd epyc
zimaboard,
laptops : puertos limitados, maximo un mini nvmeen lugar de la tarjeta de red, un disco duro en el puerto ata de dvd drive, maximo 2.5 gb ethernet apartir de usb 3.0 , puertos usb limite de hubs sin energia externa 

los firewalls son inecesarios 

nginx superior a apache

conteiners:
docker, porteiner, conteinerd

virtuaslizar:
proxmox, qubes, QEMU

---

# aprender más de linux:
[wikibooks](https://en.wikibooks.org/wiki/Linux_Guide/How_Linux_Works)
[linux journey](https://linuxjourney.com/)
[endevoarOs wiki](https://discovery.endeavouros.com/)
[hack the box](https://www.hackthebox.com/blog/learn-linux)
[linux foundation curse](https://training.linuxfoundation.org/training/introduction-to-linux/)
[wikipedia linux portal](https://en.wikipedia.org/wiki/Portal:Linux)
[arch wiki](https://wiki.archlinux.org/)
[gentoo wiki](https://wiki.gentoo.org/wiki/Main_Page)

# youtubers de linux que recomiendo
- [The linux experiment: noticias semanales](https://yewtu.be/channel/UC5UAwBUum7CPN5buc-_N1Fw)
- [DistroTube: reviews de distros, opiniones y tutoriales](https://yewtu.be/channel/UCVls1GmFKf6WlTraIb_IaJg)
- [Luke Smith: opiniones, recomendaciones y tutoriales ](https://yewtu.be/channel/UC2eYFnH61tmytImy1mTYvhA)
- [Mental Outlaw: opiniones y noticias](https://yewtu.be/channel/UC7YOGHUfC1Tb6E4pudI9STA)
- [Michael Horn: tips de linux](https://yewtu.be/channel/UC1s1OsWNYDFgbROPV-q5arg)
- [Wolfgang's: servidores](https://yewtu.be/channel/UCsnGwSIHyoYN0kiINAGUKxg)
- [Hardware Haven: servidores](https://yewtu.be/channel/UCgdTVe88YVSrOZ9qKumhULQ)
- [y más](https://yewtu.be/watch?v=NybbsnDT5NI&t=316s)
---

# Referencias

---

<style scoped>{font-size: 21px;}</style>

- GeeksforGeeks. (2019). *Linux Tutorials | Getting Started | Introduction | GeeksforGeeks* [Video]. https://yewtu.be/watch?v=0EDwEQoui_g
- GNU. (2023). *GNU General Public License, version 2*. https://www.gnu.org/licenses/old-licenses/gpl-2.0.html
- Opensource.com. (s.f.). *What is Linux?*. https://opensource.com/resources/linux
- Opensource.com. (s.f). *What is open source?*.https://opensource.com/resources/what-open-source
- Open Source Initiative. (2007). *The Open Source Definition*. https://opensource.org/osd/
- Red Hat. (2019). *What is the Linux kernel?*. https://www.redhat.com/en/topics/linux/what-is-the-linux-kernel 
- Roch, B. (2004). *Monolithic kernel vs. Microkernel*. https://web.cs.wpi.edu/~cs3013/c12/Papers/Roch_Microkernels.pdf 
- The Linux Kernel Organization. (2019). *Is Linux Kernel Free Software?*. https://www.kernel.org/category/faq.html
- Britannica, T. Editors of Encyclopaedia (2023). *Linux*. Encyclopedia Britannica. https://www.britannica.com/technology/Linux
- Fireship. (2022). *Linux in 100 Seconds* [Video]. YouTube. https://yewtu.be/watch?v=rrB13utjYV4
- The Linux Information Project. (2006). *What is Linux?*. http://www.linfo.org/newbies.html
- The Linux Kernel Organization. (2019). *About Linux Kernel*. https://www.kernel.org/linux.html
- Wheeler, D. (2003). *History of Unix, Linux, and Open Source / Free Software*. https://tldp.org/HOWTO/Secure-Programs-HOWTO/history.html
- Michael Tunnell. (2023). *Explaining Linux Family Trees: Why Are There So Many Linux Distros?* [Video]. https://yewtu.be/watch?v=kF8CRt05s6A

---

<style scoped>{font-size: 21px;}</style>

- The Linux Information Project. (2005). *Flavors of UNIX Definition*. http://www.linfo.org/flavors.html
- Adekotujo, A., Odumabo, A., Adedokun, A., & Aiyeniko, O. (2020). *A Comparative Study of Operating Systems: Case of Windows, UNIX, Linux, Mac, Android and iOS*. https://www.researchgate.net/profile/Adedoyin-Odumabo/publication/343013056_A_Comparative_Study_of_Operating_Systems_Case_of_Windows_UNIX_Linux_Mac_Android_and_iOS/links/61f2b50a9a753545e2fe8300/A-Comparative-Study-of-Operating-Systems-Case-of-Windows-UNIX-Linux-Mac-Android-and-iOS.pdf
- The Open Group. (2008). *The Single UNIX Specification, Version 4*. https://unix.org/version4/overview.html
- IEEE. (2017). *IEEE Std 1003.1™-2017*. https://pubs.opengroup.org/onlinepubs/9699919799/
SUSE. (s.f.). *Linux Distribution*. https://www.suse.com/suse-defines/definition/linux-distribution/ 
- ezeelinux. (2018). *Linux Distributions Deconstructed*. https://www.ezeelinux.com/news/linux-distributions-deconstructed/
- Linus Torvalds. (1997). *Linux: a Portable Operating System*. https://www.cs.helsinki.fi/u/kutvonen/index_files/linus.pdf
- freeBSD. (2023). *Explaining BSD*. https://docs.freebsd.org/en/articles/explaining-bsd/
- intel. (2017). *What is Intel® Management Engine?*. https://www.intel.com/content/www/us/en/support/articles/000008927/software/chipset-software.html
- coreboot. (2017). *1. AMD Platform Security Processor (PSP) Firmware Integration Guide*. https://doc.coreboot.org/soc/amd/psp_integration.html#platform-security-processor-psp-overview  
- dayzerosec. (2023). *Reversing the AMD Secure Processor (PSP) - Part 1: Design and Overview*. https://dayzerosec.com/blog/2023/04/17/reversing-the-amd-secure-processor-psp.html
- The Linux Experiment. (2018). *Linux DISTRIBUTION: explained* [Video]. https://yewtu.be/watch?v=6gqLWTSz6ck
- linuxfoundation. (2015). *Filesystem Hierarchy Standard*. https://refspecs.linuxfoundation.org/FHS_3.0/fhs-3.0.html
- creativecommons. (s.f). *About The Licenses*. https://creativecommons.org/licenses/
- GNU. (s.f). *What is Free Software?*. https://www.gnu.org/philosophy/free-sw.html
- opensource initiative. (s.f). *OSI Approved Licenses*. https://opensource.org/licenses/
- Eric Steven Raymond. (2003). *Basics of the Unix Philosophy*. http://www.catb.org/~esr/writings/taoup/html/ch01s06.html

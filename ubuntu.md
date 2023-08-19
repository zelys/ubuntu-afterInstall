# ¿Qué tienes que hacer después de instalar la última versión de Ubuntu Linux?

## 1.-Actualizar el sistema y todos sus paquetes

Abrimos Terminal y escribimos lo siguiente para actualizar a las últimas versiones:

```bash
sudo apt-get update && sudo apt-get upgrade
```

Luego puedes limpiar un poco el sistema con un sencillo comando:

```bash
sudo apt autoremove
```

## 2.-Instalamos todo aquello que no viene por defecto en Ubuntu ( posibilidad de reproducir mp3, avi, flash videos etc..)

No es imprescindible, pero siempre puede ayudar en determinadas situaciones, sobre todo si quieres ver archivos MPEG4, AVI o MP4.

```bash
sudo apt-get install ubuntu-restricted-extras
```

## 3.-Desactivar los resultados de búsqueda en el tablero

Una función un tanto engorrosa que solo nos «ensucia» las búsquedas en nuestro equipo. Tenemos que ir a «Configuración del sistema» > «Seguridad y privacidad» > «Búsqueda» y desactivarlo.

## 4.-Activar el Firewall de Ubuntu ufw

Solo tenemos que poner lo siguiente en Terminal:

```bash
sudo ufw enable
```

o podemos instalar la interfaz gráfica GUFW con:

```bash
sudo apt-get install gufw
```

Muy sencilla de usar, sobre todo para saber que reglas tenemos establecidas

## 5.-Explorar GNOME desktop

Ubuntu 18.04 viene con el escritorio GNOME muy especial, con funcionalidades de GNOME y de Unity. Los cambios son notables frente a Unity, asi que tómatelo con calma.

Puedes instalar sus extensiones para mejorar sus funcionalidades o cambiar sus opciones con GNOME Tweak Tool:

```bash
sudo apt install gnome-tweak-tool
```

## 6.-Instalar el gestor de paquetes Synaptic

Una de las mejores opciones para mantener actualizado el sistema es utilizar el gestor de paquetes «Synaptic Package Manager». Vamos al Terminal y ponemos:

```bash
sudo apt-get install synaptic
```

## 7.-Instalamos Wine, PlayOnLinux y VirtualBox

Con estas tres aplicaciones vamos a poder utilizar programas de Windows en nuestro Linux. No hace falta instalar las tres: Wine + PlayOnLinux (crea una capa de compatibilidad en el propio Ubuntu por lo que podremos ejecutar programas Windows directamente) o Virtualbox (programa de virtualización donde podremos instalar el Sistema Operativo Windows).

```bash
sudo apt-get install wine
sudo apt-get install playonlinux
sudo apt-get install virtualbox
```

## 8.-Instalar Preload

Básicamente Preload realiza un monitoreo de las aplicaciones que usas, y mediante el análisis de estos datos, predice qué aplicaciones ejecutas más a menudo para favorecer un arranque más rápido de las mismas. Puede mejorar drásticamente el rendimiento general de Ubuntu.

```bash
sudo apt-get install preload
```

## 9.-Instalar algunas aplicaciones fundamentales

- VLC (reproductor multimedia): `sudo apt-get install vlc`

- Programas para descomprimir todo tipo de archivos: `sudo apt-get install unace unrar zip unzip p7zip-full p7zip-rar sharutils rar uudeview mpack arj cabextract file-roller`

- Dropbox (almacenamiento online): [www.dropbox.com](https://www.dropbox.com/install?os=lnx)

- Gimp (editor de imagenes): `sudo apt-get install gimp gimp-data gimp-plugin-registry gimp-data-extras`

- Instalar el navegador Chromium: [download-chromium.appspot.com](https://download-chromium.appspot.com/)

Puedes consultar las mejores apps para Ubuntu Linux en: [10 programas imprescindibles para Linux (Ubuntu y demás distribuciones)](https://algoentremanos.com/10-programas-imprescindibles-para-linux/).

Si quieres acceder a más apps, puedes instalar Flatpak, el sistema de apps de Fedora, y tener todas sus aplicaciones directamente en el centro de software de Ubuntu:

```bash
sudo apt install flatpak
sudo apt install gnome-software-plugin-flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

## 10.-Instalar una buena aplicación para hacer backups del sistema

[Systemback](https://launchpad.net/systemback) (para copias de seguridad del sistema y restaurar posteriormente las aplicaciónes).

[Timeshift](https://teejeetech.com/timeshift/) (similar al sistema de Windows o el Time Machine de Mac).

Nota: Puedes hacer muchas más cosas, algunas de las cuales las indican en: [Things To Do After Installing Ubuntu](https://fosspost.org/things-to-do-after-installing-ubuntu/#3_Install_GNOME_Tweak_Tool).

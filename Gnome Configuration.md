<center><h1>Gnome Configuration</center></h1>

---

## Gnome Version: 45

Gnome Window-Manager: Wayland

<font>
Gnome Theme: [Magnetic](https://github.com/vinceliuice/Magnetic-gtk-theme)
</font>

<font size="2">

* Configuration Command: ```` ./install.sh -c dark -l --tweaks dracula outline --libadwaita ````
* Problems: Not all application corners have overflow hidden.
	* Add ````export GTK_THEME=Magnetic-Dark-Dracula```` in /etc/enviroment if some apps wont apply the theme
* Use Flatseal for Flatpak apps
	* add ````~/.themes```` under Filesystem
	* add GTK_THEME=Magnetic-Dark-Dracula under <i>Enviroment</i> -> <i>Variables</i>

</font>

Firefox Configuration

* make sure to use Wayland
	* add ````MOZ_ENABLE_WAYLAND=1```` in ````/etc/enviroment/````
* use [Firefox Gnome-Theme](https://github.com/rafaelmardojai/firefox-gnome-theme)
* colors customizable in theme/colors/*

<font>
7.1 Virtual Sourround Sound
</font>

* Copy ````/usr/share/pipewire/pipewire.conf```` to ````~/.config/pipewire```` 
* add content from [context.modules](https://gitlab.freedesktop.org/pipewire/pipewire/-/blob/master/src/daemon/filter-chain/sink-virtual-surround-7.1-hesuvi.conf) into the ````pipewire.conf````
* Download a convolver file with .wav format and replace it with ````hrir_hesuvi/hrir.wav```` (use full path to specify) in pipewire.conf
* reboot PC

<font>
App List:
</font>

* [Clapper](https://github.com/Rafostar/clapper) - A GNOME media player
* [ProtonPlus](https://github.com/Vysp3r/ProtonPlus) - Downloads Custom Proton Versions
* [Extension Manager](https://github.com/mjakeman/extension-manager) - Client for the installation of extensions from extensions.gnome.org
* [Steam](https://store.steampowered.com) - Game provider
* [Heroic Games Launcher](https://heroicgameslauncher.com/) - Linux Client to install Games from GOG, Epic Games and Prime Gaming

<font>
Extension List:
</font>

* [gnome-ext-hanabi](https://github.com/jeffshee/gnome-ext-hanabi) - Gnome extension for Live Wallpaper
	* Installation: ````run.sh install````
* [Blur my Shell](https://github.com/aunetx/blur-my-shell) - Gnome extension for optimizing the Gnome look
* [Caffeine](https://github.com/ben-manes/caffeine) - Gnome extension to prevent screensaver from quick menu if needed
* [Code - OSS](https://github.com/microsoft/vscode) - IDE
* [Impression](https://apps.gnome.org/de/Impression/) - to make bootable USBs
* [PDF Arranger](https://github.com/pdfarranger/pdfarranger) manipulates PDF files

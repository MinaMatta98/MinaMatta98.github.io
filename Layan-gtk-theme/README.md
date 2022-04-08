## Layan-gtk-theme

Layan is a flat Material Design theme for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments like Gnome, Budgie, etc.

This theme is based on materia gtk theme of nana-4. Thanks nana-4 sincerely for his great job!

All thanks to the original author of the finalised package:
**https://github.com/vinceliuice/Layan-gtk-theme**, 
and the original creator of the theme: **materia gtk theme: https://github.com/nana-4/materia-theme**

## Previews
![1](https://cn.opendesktop.org/img/5/d/3/a/7a86d212835c855e62ca9725c0031e6202ae.jpg)
![2](https://cn.opendesktop.org/img/a/1/c/3/29262c8cf691666cca24a0636d22506daaca.jpg)
![3](https://cn.opendesktop.org/img/7/a/8/7/26cacc08dc680e481f806e2626da080ab9fd.png)
![4](https://cn.opendesktop.org/img/e/a/a/1/039563371d380c59ba9ad7d0a2b3cd6ebb00.jpg)

## Info

### GTK+ 3.20 or later

### GTK2 engines requirment
- GTK2 engine Murrine 0.98.1.1 or later.
- GTK2 pixbuf engine or the gtk(2)-engines package.

Fedora/RedHat distros:

    dnf install gtk-murrine-engine gtk2-engines

Ubuntu/Mint/Debian distros:

    sudo apt-get install gtk2-engines-murrine gtk2-engines-pixbuf

ArchLinux:

    pacman -S gtk-engine-murrine gtk-engines

Other:
Search for the engines in your distributions repository or install the engines from source.

## Install Or Uninstall

Open the terminal at current directory.

Run

    ./install.sh

### On Snapcraft

<a href="https://snapcraft.io/layan-themes">
<img alt="Get it from the Snap Store" src="https://snapcraft.io/static/images/badges/en/snap-store-black.svg" />
</a>

You can install the theme from the Snap Store оr by running:

```
sudo snap install layan-themes
```
To connect the theme to an app run:
```
sudo snap connect [other snap]:gtk-3-themes layan-themes:gtk-3-themes
```
To connect the theme to all apps which have available plugs to gtk-common-themes you can run:
``` 
for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i layan-themes:gtk-3-themes; done
```

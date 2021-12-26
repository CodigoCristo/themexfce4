# Tema para Xfce4 Arcris

Tema para Xfce4


### Programas extras 📋

_Que cosas necesitas para instalar tema_

```
yay -S plata-theme-bin --noeditmenu --noconfirm --needed
```
```
yay -S papirus-icon-theme --noeditmenu --noconfirm --needed
```
```
yay -S gtk-engine-murrine --noeditmenu --noconfirm --needed
```
```
yay -S ttf-roboto --noeditmenu --noconfirm --needed
```
```
yay -S pavucontrol --noeditmenu --noconfirm --needed
```
```
yay -S gedit --noeditmenu --noconfirm --needed
```
```
yay -S gedit-plugins --noeditmenu --noconfirm --needed
```
```
yay -S plank --noeditmenu --noconfirm --needed
```
```
yay -S plank-theme-namor --noeditmenu --noconfirm --needed
```

### Instalación: 

```
git clone https://github.com/CodigoCristo/themexfce4.git
cd themexfce4
unzip -o configxfce4.zip -d ~/
unzip -o glorius.zip -d /usr/share/lightdm-webkit/themes/
```

### Instalación de Lightdm: 
```
sed -i 's/^webkit_theme\s*=\s*\(.*\)/webkit_theme = glorious #\1/g' /etc/lightdm/lightdm-webkit2-greeter.conf
sed -i 's/^debug_mode\s*=\s*\(.*\)/debug_mode = true #\1/g' /etc/lightdm/lightdm-webkit2-greeter.conf
sed -i 's/#greeter-session=example-gtk-gnome/greeter-session=lightdm-webkit2-greeter/g' /etc/lightdm/lightdm.conf
```

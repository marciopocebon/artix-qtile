# artix-qtile
Automatic Qtile config to Artix
# Install
```sh
pacman -S xorg displaymanager-openrc sudo git feh numlockx setxkbmap dunst compton termite qtile rofi wget
```

# Basic configuration
```sh
$ mkdir -p ~/.config/qtile
cp /usr/share/doc/qtile*/default_config.py ~/.config/qtile/config.py
# ou: wget -q git.io/qtile.py -O ~/.config/qtile/config.py
python -m py_compile config.py
```
# Shortcuts
+ Logout - **Super + Ctrl + q**
+ Restart - **Super + Ctrl + r**
+ Close window - **Super + w**
+ Switch window - **Super + space**
+ Two windows side by side - **Super + tab**

# Custom configuration
+ Dependencies
> Font Fantasque
```sh
$ git clone https://github.com/terroo/fonts
mkdir -p ~/.local/share
mv fonts/fonts ~/.local/share/
fc-cache -fv
```

+ install
```sh
$ git clone https://github.com/artix-qtile
cd artix-qtile
cp config.py startup ~/.config/qtile/
cd ~/.config/qtile
python2 -m py_compile config.py
# or
python -m py_compile config.py
```

+ start
```sh
$ cat <<EOF > ~/.xinitrc
exec qtile
EOF
startx
```


# artix-qtile
Automatic Qtile config to Artix
# Install
```sh
pacman -S qtile termite
```

# Basic configuration
```sh
mkdir -p ~/.config/qtile
cp /usr/share/doc/qtile*/config.py ~/.config/qtile
# ou
wget -q git.io/qtile.py -O ~/.config/qtile/config.py
python -m py_compile config.py
```
# Shortcuts
+ Logout - **Super + Ctrl + q**
+ Restart - **Super + Ctrl + r**

# Custom configuration
+ Dependencies
```sh
git feh numlockx setxkbmap dunst compton termite
```
> Font Fantasque

+ install
```sh
git clone https://github.com/artix-qtile
cd artix-qtile
cp config.py startup ~/.config/qtile/
cd ~/.config/qtile
python2 -m py_compile config.py
```

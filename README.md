# Bootstrap Script

![Mountain Background](./mountain.jpg)

```
echo "DE: Xfce4"
echo "WM: Xfwm4"
echo "WM Theme: Numix"
echo "GTK Theme: Numix [GTK2]"
echo "Icon Theme: Papirus"
echo "Font: Cantarell 9"
```

## Prepare home

```
cd ~
mkdir ~/dev
mkdir ~/dev/bin
```

## Linux tools

```
sudo pacman -Sy curl
sudo pacman -Sy bat
sudo pacman -Sy tree
sudo pacman -Sy htop
sudo pacman -Sy the_silver_searcher
sudo pacman -Sy docker
sudo pacman -Sy terminator
sudo pacman -Sy git
sudo pacman -Sy neovim
sudo pacman -Sy flatpak
sudo pacman -Sy ranger
sudo pacman -Sy fzf
sudo pacman -Sy ncdu
sudo pacman -Sy ctop
sudo pacman -Sy httpie
sudo pacman -Sy xsel
sudo pacman -Sy tldr
sudo pacman -Sy screenfetch
sudo pacman -Sy rofi
sudo pacman -Sy aws-cli
sudo pacman -Sy inotify-tools
sudo pacman -Sy postgresql
sudo pacman -S noto-fonts-emoji
```

## Numix Theme

According https://github.com/numixproject/numix-gtk-theme#build-it

```
git clone git@github.com:numixproject/numix-gtk-theme.git
cd numix-gtk-theme

sudo pacman -S sassc glib2 gdk-pixbuf2

sudo make install

xfconf-query -c xsettings -p /Net/ThemeName -s "Numix"
xfconf-query -c xfwm4 -p /general/theme -s "Numix"
```

## Other tools

### asdf

```
git clone https://github.com/asdf-vm/asdf.git ~/.asdf
cd ~/.asdf
git checkout "$(git describe --abbrev=0 --tags)"
```

### heroku

```
curl https://cli-assets.heroku.com/install.sh | sh
```

### ngrok

```
echo "Download from https://ngrok.com/download and follow instructions" && read
```

### rpx

```
wget https://raw.githubusercontent.com/andrewaguiar/rpx/master/bin/rpx
chmod +x rpx
mv rpx ~/dev/bin
```

## Dotfiles

### bashrc, bash_profile, neovimfiles

```
cd ~
git clone git@github.com:andrewaguiar/dotfiles.git
git clone git@github.com:andrewaguiar/neovimfiles.git
```

## Other softwares

```
pamac install firefox
pamac install chromedriver
pamac install google-chrome
pamac install thunar
pamac install dropbox
flatpak install us.zoom.Zoom
flatpak install org.signal.Signal
flatpak install com.slack.Slack
flatpak install com.skype.Client
flatpak install org.gnome.Cheese
flatpak install flathub com.belmoussaoui.Authenticator
flatpak install flathub com.getpostman.Postman
```

```
echo "Balena Etcher flash os images: https://www.balena.io/etcher/"
```

## Copy some configs to home

```
cp HOME/config/rofi ~/.config/rofi
cp HOME/config/gtk-3.0 ~/.config/gtk-3.0
cp HOME/config/terminator ~/.config/terminator
```

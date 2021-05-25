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
sudo pacman -Sy \
  curl \
  tree \
  htop \
  ag \
  docker \
  git \
  neovim \
  flatpak \
  ncdu \
  ctop \
  screenfetch
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
```

```
echo "Balena Etcher flash os images: https://www.balena.io/etcher/"
```


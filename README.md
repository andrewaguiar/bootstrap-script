# Bootstrap Script

## Install

```
cd ~
mkdir ~/dev
mkdir ~/dev/bin
```

### - Linux tools

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
  screenfetch
```

### Other tools

#### asdf

```
git clone https://github.com/asdf-vm/asdf.git ~/.asdf
cd ~/.asdf
git checkout "$(git describe --abbrev=0 --tags)"
```

#### heroku

```
curl https://cli-assets.heroku.com/install.sh | sh
```

#### ngrok

```
echo "Download from https://ngrok.com/download and follow instructions" && read
```

#### rpx

```
wget https://raw.githubusercontent.com/andrewaguiar/rpx/master/bin/rpx
chmod +x rpx
mv rpx ~/dev/bin
```

### Dotfiles

#### bashrc, bash_profile, neovimfiles

```
cd ~
git clone git@github.com:andrewaguiar/dotfiles.git
git clone git@github.com:andrewaguiar/neovimfiles.git
```

### Other softwares

```
pamac install firefox
pamac install chromedriver
pamac install google-chrome
pamac install thunar
flatpak install us.zoom.Zoom
flatpak install org.signal.Signal
flatpak install com.slack.Slack
flatpak install com.skype.Client
flatpak install org.gnome.Cheese
```

#### 1. arch-hyprland

[hyprdots](https://github.com/prasanthrangan/hyprdots)

#### 2. reflector

```shell
sudo pacman -S reflector
reflector --country China --age 72 --sort rate --protocol https --save /etc/pacman.d/mirrorlist
```

#### 2. archlinuxcn

```/etc/pacman.conf
[archlinuxcn]
SigLevel = Optional TrustAll
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinuxcn/\$arch
```

#### 2. openssh

```shell
ssh-keygen -t rsa
cat ~/.ssh/id_rsa.pub
```

#### 2. Pacman packages

zsh
openssh
stow
bat
lazygit
plocate
zathura
lf
joshuto
kitty
dunst
wofi
nsxiv
ripgrep
autojump
btop
grim
swappy
slurp
xsel
xclip
trash-cli
github-cli
neofetch
fastfetch
ttf-jetbrains-mono-nerd
ttf-firacode-nerd
ttf-jetbrains-mono-nerd
ttf-linux-libertine
ttf-ibm-plex
udiskie
numlockx
ffmpegthumbnailer
vivid
libreoffice
okular
atool
nodejs
npm
mpv
mpc
mpd
ncmpcpp
redis
kdenlive
breeze
blender
gimp
scribus
helix

#### 3. Yay Packages

swappy
swww
swaylock
google-chrome
ttf-times-new-roman
rar
qqmusic-bin
obs-studio
transmission-remote-gui


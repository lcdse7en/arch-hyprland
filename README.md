<!-- Install archlinux: archinstall -->

#### 1. arch-hyprland

[install-hyprland](https://github.com/JaKooLit/Hyprland-v3)
[hyprland-config](https://github.com/prasanthrangan/hyprdots)

#### 2. reflector

```shell
sudo pacman -S reflector
reflector --country China --age 72 --sort rate --protocol https --save /etc/pacman.d/mirrorlist
```

#### 3. archlinuxcn

```/etc/pacman.conf
[archlinuxcn]
SigLevel = Optional TrustAll
Server = https://mirrors.tuna.tsinghua.edu.cn/archlinuxcn/\$arch
```

#### 3. openssh

```shell
ssh-keygen -t rsa
cat ~/.ssh/id_rsa.pub
```

#### 4. Pacman packages

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
mako
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
ttf-fira-code
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

#### 5. Yay Packages

swappy
swww
swaylock
google-chrome
ttf-times-new-roman
rar
qqmusic-bin
obs-studio
transmission-remote-gui

<!-- Install archlinux: archinstall -->

#### 1. arch-hyprland

[install-hyprland](https://github.com/kshitijdhara/Arch-hyprland)
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

#### 4. sudoers

```shell
sed -i 's/^# %wheel ALL=(ALL) ALL/%wheel ALL=(ALL:ALL) ALL/' /etc/sudoers
sed -i 's/^# %wheel ALL=(ALL:ALL) NOPASSWD: ALL%/%wheel ALL=(ALL:ALL) NOPASSWD: ALL/' /etc/sudoers
```

#### 3. openssh & gitconfig

```shell
ssh-keygen -t rsa
cat ~/.ssh/id_rsa.pub

git config --global user.name lcdse7en
git config --global user.email 2353442022@qq.com
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
ueberzugpp
joshuto
kitty
wezterm
cronie
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
cava
pamixer
ncmpcpp
redis
kdenlive
breeze
blender
gimp
scribus
helix
odt2txt
transmission-cli
gnumeric

#### 5. Yay Packages

oh-my-zsh-git
zsh-theme-powerlevel10k-git
zsh-syntax-highlighting-git
zsh-autosuggestions-git
pokemon-colorscripts-git

```shell
chsh -s $(which zsh)
```

pamac-aur
kde-rounded-corners
latte-dock-git
spotify-adblock
spicetify-cli
spicetify-themes-git
goverlay

swappy
swww

<!-- swaybg -->

swaylock
dolphin
google-chrome
ttf-times-new-roman
rar
qqmusic-bin
obs-studio
transmission-remote-gui

#### 6. fonts

```shell
mkdir ~/.local/share/fonts/
tar -xvzf ~/dotfiles/source/fonts/Font_CascadiaCove.tar.gz -C ~/.local/share/fonts/
tar -xvzf ~/dotfiles/source/fonts/Font_MononokiNerd.tar.gz -C ~/.local/share/fonts/
tar -xvzf ~/dotfiles/source/fonts/Font_JetBrainsMono.tar.gz -C ~/.local/share/fonts/
sudo tar -xvzf ~/dotfiles/source/fonts/Font_UzumasaMini.tar.gz -C /usr/share/fonts/

fc-cache -vf
fc-list
```

#### 7. sddm

```shell
tar -xvzf ~/dotfiles/source/fonts/Sddm_Corners.tar.gz -C -C /usr/share/sddm/themes/
sudo cp /etc/sddm.conf.d/kde_settings.conf /etc/sddm.conf.d/kde_settings.bkp
sudo sed -i "/^Current=/c\Current=corners" /etc/sddm.conf.d/kde_settings.conf
```

#### rofi

```shell
sudo cp ~/dotfiles/rofi/.config/rofi/cat_*.rasi /usr/share/rofi/themes/
```

#### 8. firefox

```shell
FoxRel=`ll ~/.mozilla/firefox/ | grep .default-release | awk '{print $NF}'`
mkdir ~/.mozilla/firefox/${FoxRel}/chrome
cp ~/dotfiles/source/t2_firefox.css ~/.mozilla/firefox/${FoxRel}/chrome/userChrome.css

// about:profiles
// about:config
 -> toolkit.legacyUserProfileCustomizations.stylesheets - true
 -> browser.tabs.tabmanager.enabled - false
```

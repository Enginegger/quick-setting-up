# quick-setting-up
быстро поставить рабочую систему на свжем пк


QUICK SETUP INSTALLATION 
```
sudo apt update -y
```
```
sudo apt install git curl wget zsh tmux alacritty neovim mc stow tldr -y
mc - midnight commander
```
alacr - console emulator
tmux - multiplexor inside the alacr
#. set oh my zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

#. do ssh-keygen twice for work and own GitHub
```
ssh-keygen -t ed25519 -C "example@gmail.com" -f ~/.ssh/id_nameService
```
#. when set ssh to the github
```
cd ~/Documents
git clone git@github.com:Enginegger/coder-notes.git
git config user.name "Enginegger"
```
`git config user.email "your-email@gmail.com" # have to change`

# dotfiles
cd 
```
rm -rf ~/.dotfiles
rm -f ~/.zshrc
git clone git@github.com:Enginegger/.dotfiles.git
cd .dotfiles
stow .
git config user.name "Enginegger"
```
`git config user.email "your-email@gmail.com"`

#. jet brains font
```
mkdir -p ~/.local/share/fonts
cd ~/.local/share/fonts
wget https://github.com/ryanoasis/nerd-fonts/releases/latest/download/JetBrainsMono.zip
unzip JetBrainsMono.zip
fc-cache -fv
```

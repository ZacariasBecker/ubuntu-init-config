# Initial Ubuntu configutation

### General
+ `sudo apt update -y`
+ `sudo apt upgrade -y`
+ `sudo apt install dkms make perl gcc build-essential git curl -y`
+ `sudo add-apt-repository ppa:deadsnakes/ppa`
+ `sudo apt install python3.10-full python3.10-dev`
+ `curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -`
+ `sudo apt-get install -y nodejs`
+ `sudo npm install --global yarn`
+ `sudo apt install fonts-firacode`

### vscode nautilus
+ `wget -qO- https://raw.githubusercontent.com/harry-cpp/code-nautilus/master/install.sh | bash`


### zsh
+ `sudo apt install zsh -y`
+ `chsh -s /bin/zsh`
+ `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
+ `git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1`
+ `ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"`
+ `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
+ `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

### Changes in ~/.zshrc
+ ZSH_THEME="spaceship"
+ plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

### Fonts
+ `mkdir -p ~/.fonts`
+ `git clone https://github.com/pdf/ubuntu-mono-powerline-ttf.git ~/.fonts/ubuntu-mono-powerline-ttf`
+ `fc-cache -vf`

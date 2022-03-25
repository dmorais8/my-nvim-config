# my-nvim-config

## Requirements

- NodeJS LTS
- Python >= 3.8
- Neovim >= 0.5.1

## Setup Environment

### Setup directory/files structure:

```
mkdir -p ~/.config/nvim
cp init.vim ~/.config/nvim
cp coc-settings.json ~/.config/nvim
```
### Install dependencies

Install Plugin manager

#### NVIM

```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

#### VIM

```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

Install Terraform-LSP

```
wget https://releases.hashicorp.com/terraform-ls/0.26.0/terraform-ls_0.26.0_linux_amd64.zip \
unzip terraform-ls_0.26.0_linux_amd64.zip \
sudo mv terraform-ls_0.26.0_linux_amd64.zip/terraform-ls /usr/local/bin/
```

Extra Packages

```
sudo apt update && sudo apt install ripgrep fd-find fzf -y
```

### Apply Config

Open nvim

```
nvim
```

Type **:PlugInstall** to install the plugins and themes.
...




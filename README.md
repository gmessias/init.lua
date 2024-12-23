# Neovim

## WSL - Ubuntu

Sistema
```
sudo apt update
sudo apt upgrade
```

```
sudo apt install build-essential curl wget git
sudo apt install unzip tar xz-utils
```

```
mkdir -p ~/.config/nvim
```

---

zsh
```
sudo apt install zsh
```

Definir como padrão
```
chsh -s $(which zsh)
```

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
```

No arquivo ~/.zshrc
> plugins=(git zsh-autosuggestions)

Ativar
```
source ~/.zshrc
```

---

Telescope

ripgrep
```
sudo apt install ripgrep
```

fd
```
sudo apt install fd-find
ln -s $(which fdfind) ~/.local/bin/fd
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

---

Clonar o repositório dentro de ~/.config/nvim

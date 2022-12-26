# Install oh-my-zsh
---
[***@nabang1010***](https://github.com/nabang1010)

## Install oh-my-zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install powerlevel10k

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

## Install Plugins

### zsh-autosuggestions


```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### zsh-syntax-highlighting

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```

### Add Plugins to `.zshrc`

- Edit `.zshrc`

```bash
sudo gedit ~/.zshrc
```
- Add plugins

```txt
plugins=(git 
        zsh-syntax-highlighting 
        zsh-autosuggestions 
        history 
        aliases 
        web-search
        )
```
- Soure

```bash
source ~/.zshrc
```
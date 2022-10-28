# Dev Enviroment Setting Upp Macbook

# Install Homebrew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Website: https://brew.sh/

# Install iTerm2
- Download: https://iterm2.com/downloads.html
- Install iTerm2 with brew:
```bash
brew install --cask iterm2
```
# Install Oh My ZSH!
- https://ohmyz.sh/#install
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Plugins
#### powerlevel10k
- [powerlevel10k](https://github.com/romkatv/powerlevel10k#installation)
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
#### zsh-autosuggestions
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
#### zsh-autosuggestions
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

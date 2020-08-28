
# ZSH-Theme - My lovely iTerm2 Terminal
![preview](https://github.com/xVanjaZ/ZSH-Theme/blob/master/preview.png)

### Download and install [iTerm2](https://www.iterm2.com)

### Install Oh My Zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Install Spaceship-Promt

```
git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```
Set `ZSH_THEME="spaceship"` in `~/.zshrc`

### Install Powerline fonts <br>

```
# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts
```

### Download The-one-theme <br>
```
git clone https://github.com/benniemosher/the-one-theme/
```

### Activating the theme and font
1. iTerm2 > Preferences  <br>
2. Profiles > Select "Default" profile  <br>
3. Colors > Color Presets > Import and select the iTerm theme  <br>
4. Text > Change Font > All fonts > Fira Mono for Powerline  <br>


### Install syntax highlighting
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
source ./zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

### Add autosuggestion
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
Set `plugins=(git zsh-autosuggestions)` in `~/.zshrc`

### Import custom settings
Copy the contents from [settings.conf](https://github.com/xVanjaZ/ZSH-Theme/blob/master/settings.conf) at the bottom of `.zshrc` <br>
More info about custom settings can be found [here](https://github.com/denysdovhan/spaceship-prompt/blob/master/docs/Options.md)

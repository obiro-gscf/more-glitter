# Terminal app configuration

1. View > Show Tab Bar


# Oh-my-zsh

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Change the theme in `~/.zshrc` to `avit` or `amuse`

## Plugins

### ZSH Autosuggestions

1. Clone this repository into `$ZSH_CUSTOM/plugins` (by default `~/.oh-my-zsh/custom/plugins`)

    ```shell
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    ```

2. Add the plugin to the list of plugins for Oh My Zsh to load (inside `~/.zshrc`):

    ```shell
    plugins=( 
        # other plugins...
        zsh-autosuggestions
    )
    ```

3. Start a new terminal session.

### ZSH Syntax Highlighting

1. Clone this repository in oh-my-zsh's plugins directory:

    ```shell
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    ```

2. Activate the plugin in `~/.zshrc`:

    ```shell
    plugins=( [plugins...] zsh-syntax-highlighting)
    ```

3. Restart zsh (such as by opening a new instance of your terminal emulator).


# Nerd font

1. Install your preferred [Nerd Font](https://www.nerdfonts.com/font-downloads)

```sh
brew tap homebrew/cask-fonts && brew install --cask font-sauce-code-pro-nerd-font
```

2. Change the font in Terminal: Settings > Profiles > Font

> Using the nerd font will allow to display more icons than with the standard fonts
# Starship

``` sh
brew install starship
```

Add the following to the end of `~/.zshrc`:

```
# ~/.zshrc

eval "$(starship init zsh)"
```

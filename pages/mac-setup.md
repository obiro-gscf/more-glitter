# Macbook setup

## Before you start

Before you start any additional configuration, make sure you go to:

System Settings > Appearance 

and change the system color scheme to Dark. This is the **only right** way.

> Please note that all the tools mentioned below have support for dark mode. Use it. Your eyes will thank you.
> 
> (And your managers will too, as it is commonly known that light themes attract bugs!)

## Useful system settings

- System Settings > Keyboard > Keyboard Shortcuts > Function Keys (enable)
- System Settings > Keyboard > Keyboard Shortcuts > Input Sources (disable, IntelliJ Classic keymap overrides these shortcuts)
- System Settings > Keyboard > Keyboard Shortcuts > Services > Text > Search man Page Index in Terminal (disable)
- System Settings > Trackpad > Tap to click (enable)


- Finder > View > Show Tab Bar
- Finder > View > Show Toolbar
- Finder > View > Show Path Bar
- Finder > View > Show Status Bar
- Finder > Cmd + Shift + . (show / hide hidden fiels)

## Essential command line tools

### Homebrew

[Homebrew](https://brew.sh) is a Mac-native command line tool for downloading and managing applications.

> If you're familiar with Linux, `brew` is Mac equivalent of `apt-get`

Useful commands:

- `brew install <app-name>` - installs the application
- `brew search <app-name>` - searches for entries by app-name
- `brew info <app-name>` - displays more information about a specific app
- `brew update` - updates the local definition of the applications to "latest"
- `brew upgrade` - upgrades the locally installed application (usually: run this *after* `brew update`)
- `brew list` - lists all installed applications

|                            |                                                                                                                                     |
|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| What are the alternatives? | - Installing applications directly from the websites <br/> - Using AppStore                                                         |
| Why use this option?       | - In most of the cases, all the apps you need can be found here<br/> - Updating *all* of your software at once, with just 1 command |

### oh-my-zsh

[Oh-My-Zsh](https://ohmyz.sh) is a framework for managing the terminal configuration. You can read more about my personal zsh setup [here](terminal-setup.md).

> If you're a power-user of command line (and / or a fan of Linux cmd capabilities), I highly recommend giving it a try. 

|                            |                                                                                                                                                            |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| What are the alternatives? | Using a standard terminal **OR** not using terminal at all.                                                                                                |
| Why use this option?       | (if you use your terminal often) It allows to (easily) configure a lot of things, i.e. custom color scheme, autosuggestions, better prompt formatting etc. |

### jEnv

[jEnv](https://www.jenv.be) is a command line tool for managing (multiple) Java versions.

|                            |                                                                                                                                                               |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| What are the alternatives? | Manually installing specific Java version(s).                                                                                                                 |
| Why use this option?       | It takes care of managing multiple Java versions, you can switch between them with just 1 command (and you never need to worry about "how to set JAVA_HOME"). |

### NVM

[NVM](https://collabnix.com/how-to-install-and-configure-nvm-on-mac-os/) is a Node Version Manager. It gives the same capabilities as [jEnv](#jenv), but for Node. 

|                            |                                                                                                         |
|----------------------------|---------------------------------------------------------------------------------------------------------|
| What are the alternatives? | Manually installing specific Node version(s).                                                           |
| Why use this option?       | It takes care of managing multiple Node versions and allows to switch between them with just 1 command. |

### awscli

The CLI for AWS - absolutely needed for connecting to AWS services.

## Essential apps

### IntelliJ

IntelliJ is an IDE for Java development, but it is also so much more. This is easily the most used app for me, and one I cannot imagine my (professional) life without.

Check out my [IntelliJ Cheatsheet](intellij-cheatsheet.md) here ;)

|                            |                                                                                                   |
|----------------------------|---------------------------------------------------------------------------------------------------|
| What are the alternatives? | - (theoretically) any other code editor<br/> - Visual Studio                                      |
| Why use this option?       | It's the best, especially for Java / Kotlin development. Once you go IntelliJ, you never go back. |

### Obsidian

[Obsidian](https://obsidian.md) is a lightweight, powerful and **FREE** note-taking app. It happens to be my top pick in terms of productivity apps. You can read a bit more about my Obsidian setup [here](obsidian-setup.md).

|                            |                                                                                                                                                                                                                                                                                                                                             |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| What are the alternatives? | - (theoretically) any other text editor<br/> - [IntelliJ](#intellij) <br/> - [Sublime Text](#sublime-text) <br/> - Notion<br/> - Bear <br/> - OneNote                                                                                                                                                                                       | 
| Why use this option?       | - you can choose to have your notes *only* on your local machine<br/> - Markdown syntax (notes are easily transferable)<br/> - clean and pretty UI<br/> - supports linking between notes<br/> - many community-supported plugins<br/> - amazing for technical notes, specifically with code snippets <br/> - as simple as you want it to be |

### Postman

[Postman](https://www.postman.com) is a graphical tool for building and using / testing APIs. It is useful for manually triggering requests to specific endpoints.

|                            |                                                 |
|----------------------------|-------------------------------------------------|
| What are the alternatives? | - `curl` <br/> - many other tools on the market |
| Why use this option?       | It is free, pretty and simple to use.           |

### Skitch

Skitch is a simple screen-capture app which also offers basic markup and sharing features. Great for taking screenshots.

|                            |                                                                                                                      |
|----------------------------|----------------------------------------------------------------------------------------------------------------------|
| What are the alternatives? | Built-in screenshot mechanism.                                                                                       |
| Why use this option?       | Who has the time to memorize all the overly-complicated screenshot keyboard shortcuts? ;) It is just simpler to use. |

### Sublime Text

[Sublime Text](https://www.sublimetext.com) is a (**FREE**) simple but very powerful text editor. I would describe it as Notepad++ on steroids. 

I use it mainly for opening configuration files / viewing and editing small code snippets or scripts; basically anything semi-technical that is too small to justify opening a new project in IntelliJ for it. 

|                            |                                                                                                                                                                                                                                                 |
|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| What are the alternatives? | - TextEdit (built-in text editor)<br/> - TextMate<br/>                                                                                                                                                                                          |
| Why use this option?       | - it has **many** plugins<br/> - it can be as powerful as vim / emacs, but is much simpler to use (as simple as you want it to be)<br/> - built-in syntax highlighting for majority of the popular languages (and many more covered by plugins) |

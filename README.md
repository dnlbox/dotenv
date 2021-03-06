# Dev Setup

## Why care about this?

As a craftsman, care about the tools you use to perform your craft it is essencial and a sign of respect for the craft.
- keep your tools clean (specially the screen);
- be familiar with the tools;
- collaborate when possible.

## MacOSX

+ to make super+tab faster on fullscreen:
  - Accessibility enable `Display > Reduce motion`

+ because dark side is more fun:
  - On General, enable `Use dark menu bar and Dock`

### Font

__Fira__: https://github.com/mozilla/Fira (no ligatures)

#### Install using Homebrew Cask Fonts (https://github.com/Homebrew/homebrew-cask-fonts)

`brew tap Homebrew/cask-fonts` (https://github.com/Homebrew/homebrew-cask/blob/master/USAGE.md)  
`brew cask install font-fira-code font-fira-mono font-fira-sans` (https://github.com/Homebrew/homebrew-cask-fonts)  

## Brew

install brew using regular terminal
- `brew install cask`
- `brew cask install iterm2`
- `brew install zsh zsh-completions zsh-syntax-highlighting antigen`
- `brew install git`
- `brew install yarn`
- `brew install ncdu` folder size inspection
- `brew install bat` cat with highlights
- `brew install tree` visualize folder structure
- `brew install ios-deploy` I don't remember why but I know that I need it
- `brew install youtube-dl` thanks expensive 4g and no train wifi
- `brew install p7zip` zip utils
- `brew install cask android-platform-tools` adb on the command line among other things
- `brew install wget`

source: [Brew](https://brew.sh/)

## iTerm

### General

- to load faster, delete Apple system logs:
`sudo rm /var/log/asl/*.asl` - sudo :unamused:

### ZSH (oh-my-zsh)

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

### Antigen

```
# Load the oh-my-zsh's library.
antigen use oh-my-zsh

# Bundles
antigen bundle tarruda/zsh-autosuggestions
antigen bundle zsh-users/zsh-syntax-highlighting

# Load the theme.
antigen theme robbyrussell

# Tell Antigen that you're done.
antigen apply
```

source: [Antigen](https://github.com/zsh-users/antigen)

### Alias

- to open iOS Simulator from the command line:
`alias ios-simulator="open /Applications/Xcode.app/Contents/Developer/Applications/Simulator.app/"`

- general alias on .bash_profile:
`alias l='ls -lh' && alias ll='ls -lah'`

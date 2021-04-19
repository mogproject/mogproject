
## Setup my Mac

### MacBook Pro 2016 (macOS Sierra)

- Initial setup
- Logging into accounts: Apple/Google

### System Preferences

- Sharing
  - Rename the computer name
- Desktop & Screen Saver
  - Screen Saver
    - Start after: 30 Minutes
    - Hot Corners
      - Top-left: Launchpad
      - Bottom-left: Start Screen Saver
- Dock
  - Size: smaller
  - Position on screen: Left
  - [x] Automatically hide and show the Dock
- Mission Control
  - [ ] Automatically rearrange Spaces based on most recent use
  - Keyboard and Mouse Shortcuts
    - Show Desktop: F11 -> "-"
    - Show Dashboard: F12 -> "-"
- Security & Privacy
  - [x] Require password: immediately
  - [x] Show a message when the screen is locked
    - Lock message: "[Emergency Contact]\nTwitter: @mogproject   Email: mogproj@gmail.com"
  - Firewall: Turn On
- Keyboard
  - Modifier Keys (only if keyboard == Apple Internal Keyboard)
    - Caps Lock -> Control
    - Control -> Caps Lock
    - Option -> Command
    - Command -> Option
- Trackpad
  - Tap to click
- Sound
  - Sound Effects
    - Internal Speakers
    - Alert volume: 0
- Users & Groups
  - Edit the icon
  - Set shell: /bin/zsh
  - Gest User: Off
- Kayboard
  - Text
    - [ ] Correct spelling automatically
    - [ ] Capitalize words automatically
    - [ ] Add period with double-space
    - [ ] Use smart quotes and dashes

- Remove unnecessary icons from Dock

### Finder

```
defaults write com.apple.finder AppleShowAllFiles YES
killall Finder
```

```
defaults write .GlobalPreferences com.apple.scrollwheel.scaling -1
```

### Firefox

- Download & install
- Advanced
  - Data Choices

### DropBox

- Download & install

```
## deprecated from 10.15 ## sudo ln -s ~/Dropbox /
```

- Install fonts
  - Essential Pragmata Pro Family

### BetterTouchTool

- Download & install
- Import license file
- Advanced Settings
  - [x] Launch BetterTouchTool on startup
- Global
  - ^M: Enter  repeat, 0.06, 0.2
  - ^I: Tab
- Define trackpad gestures


### Homebrew

- Install Homebrew

```
brew install tmux
ln -s ~/Dropbox/config/_tmux.conf ~/.tmux.conf
```

```
brew install htop pyenv npm tig
```

### iTerm2

- Download & install
- Preferences
  - Closing
    - [ ] Confirm closing multiple sessions
    - [ ] Confirm "Quit iTerm2" command
- Hotkey
- Create Visor profile
  - General
    - Name: Visor
    - Command: Send text at start: tmux a || tmux
  - Colors: Load "SolarizedHighContrastDark"
  - Text: Font-> Essential PragmataPro, NON-ASCII -> Osaka-Mono
  - Window:
    - Set transparency
    - Style: Full-Width Top of Screen
  - Terminal
    - Silence bell, flash visual bell -> Off
  - Session
    - Prompt before ...
  - Keys: Left/Right option -> Esc+  !!! IMPORTANT !!!
    - Hotkey: ^`

- Create `~/.zshrc`

```
. /Dropbox/config/_zshrc
```

```
$ cd /usr/local/share/
$ sudo chmod -R 755 zsh
$ sudo chown -R root:staff zsh
```

- Install JDK

### TotalSpaces2

- Download & install
- Register the license
- General
  - Start at Login
  - Zoom to overview grid animation: None
  - Backgrounds in the overview grid: None (fastest)
- Layout: 9x9
- Transitions: the Fastest

### [Deprecated!] Karabiner-Elements

- Key Repeat
  - Delay: 250 ms
  - Key Repeat: 20 ms

### Key Repeat Setting (new)

```
defaults write -g InitialKeyRepeat -int 20
defaults write -g KeyRepeat -int 1
```

### Key bindings

```
mkdir ~/Library/KeyBindings
ln -s $DROPBOX_DIR/config/_EmacsKeyBinding.dict ~/Library/KeyBindings/DefaultKeyBinding.dict
```

### Programming Languages

#### Python

```
brew install readline xz
sudo installer -pkg /Library/Developer/CommandLineTools/Packages/macOS_SDK_headers_for_macOS_10.14.pkg -target /
pyenv install 2.7.15

pip install pep8
```

#### Misc

```
brew install coreutils clang-format
````

- [ ] git / [GitHub](github.md)
- [ ] Vim: `echo ":source /Dropbox/config/_vimrc" > ~/.vimrc`
- [ ] [f.lux](https://justgetflux.com/)
- [ ] [Firefox](firefox.md)
- [ ] [Visual Studio Code](vscode.md)
- [ ] [Scroll Reverser](https://pilotmoon.com/scrollreverser/)
- [ ] Logicool Mouseware
- [ ] Skitch (App Store)
- [ ] iTunes: library data migration



##### Old Link

- ref. https://github.com/mogproject/mogproject/wiki/Setup-My-Mac


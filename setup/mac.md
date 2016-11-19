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
  - Modifier Keys
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

- Remove unnecessary icons from Dock

### Firefox

- Download & install
- Advanced
  - Data Choices

### DropBox

- Download & install

```
sudo ln -s ~/Dropbox /
```

- Install fonts
  - Essential Pragmata Pro Family

### BetterTouchTool

- Download & install
- Import license file
- Advanced Settings
  - [x] Launch BetterTouchTool on startup
- Define trackpad gestures

### iTerm2

- Download & install
- Preferences
  - Closing
    - [ ] Confirm closing multiple sessions
    - [ ] Confirm "Quit iTerm2" command
- Hotkey
- Create Visor profile
- Import "Solalized Dark Higher Contrast" color preset

- Create `~/.zshrc`

```
. /Dropbox/config/_zshrc
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

### Homebrew

- Install Homebrew

```
brew install tmux
ln -s /Dropbox/config/_tmux.conf ~/.tmux.conf
```

### Karabiner-Elements

- Key Repeat
  - Delay: 250 ms
  - Key Repeat: 20 ms


### Key bindings

```
mkdir ~/Library/KeyBindings
ln -s $DROPBOX_DIR/config/_EmacsKeyBinding.dict ~/Library/KeyBindings/DefaultKeyBinding.dict
```

- [ ] Flash Player
- [ ] [GitHub](github.md)
- [ ] Vim: `echo ":source /Dropbox/config/_vimrc" > ~/.vimrc`
- [ ] [f.lux](https://justgetflux.com/)
- [ ] [Firefox](firefox.md)

##### Old Link

- ref. https://github.com/mogproject/mogproject/wiki/Setup-My-Mac



### Visual Studio Code

- Download & install the binary
- User settings
  - `~/Library/Application\ Support/Code/User/keybindings.json`
  - `~/Library/Application\ Support/Code/User/settings.json`
  - `~/Library/Application\ Support/Code/User/snippets/cpp.json`
- Install extensions
  - C++ by Microsoft
  - Python by Don Jayamanne
  - Python Extended by Taiwo Kareem
  - TODO Parser by minhtai
  - [mog-vscode](https://github.com/mogproject/mog-vscode)


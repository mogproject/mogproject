## Set up `lecture` account on Mac

8/30/2021

### System Preferences

- Dock: move the Dock to the left
- Mission Control: hot corners
- Desktop: color #3c6ea6
- Keyboard: modifier keys: Caps Lock -> Control
- Mouse: disable Scroll direction Natural

### Firefox

- Log into GitHub, Kahoot
- Edit `about:config`: https://github.com/mogproject/mogproject/blob/master/setup/firefox.md
- Add-on
  - Group Speed Dial
  - Set homepage, etc.

### Fonts

- Install Essential Pragmata Pro

### iTerm2

- Configure `Visor` profile

### SoundSource

- Licensing

### SSH

- Set up `~/.ssh`

### Zsh

- Set up `~/.zshrc`

### Git

- Set up `~/.gitconfig`

### Mini-conda

```
conda init zsh
conda create -n lecture python=3.9
conda install jupyterlab plotly
```
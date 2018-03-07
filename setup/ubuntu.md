Set up my Ubuntu

- ubuntu 16.04 LTS


## Keyboard Preference

- Open Terminal (Ctrl + Alt + T)
- `sudo apt install gnome-tweak-tool`
- `gnome-tweak-tool`
  - Typing -> Swap Ctrl and Caps Lock

- System Settings
  - Sound -> Sound Effects: Mute
  - Mouse & Touchpad -> Natural scrolling: On

- Install Dropbox

```
sudo ln -s ~/Dropbox /
```

- Diable guest session

- `sudo vi /usr/share/lightdm/lightdm.conf.d/50-ubuntu.conf`
- Add `allow-guest=false`

- Install software tools

```
sudo -i

apt install tmux
add-apt-repository ppa:gnome-terminator
apt-get update
apt-get install terminator
```



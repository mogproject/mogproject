Setup Firefox
====

### about:config

- browser.search.openintab: false => true
- browser.tabs.closeWindowWithLastTab: true => false
- browser.tabs.warnOnClose: true => false
- mousewheel.default.delta_multiplier_y: 100 => 400
- mousewheel.min_line_scroll_amount: 5 => 40

### policies.json

- Create directory: `/Applications/Firefox.app/Contents/Resources/distribution`
- Create file: `policies.json`

```
{
"policies": 
   {
     "DisableAppUpdate": true
    }
}
```



### Add-ons

##### YesScript

- Blacklist

```
http://www.google.com
https://www.google.com
```

##### In My Pocket
##### Make Link
##### Open Link in New Tab
##### Speed Dial

- Options
  - [x] Load in blank new windows
  - [x] Load in blank new tabs
  - [x] Enable dial groups
  - [x] Add Speed Dial button to toolbar
  - [x] Set Speed Dial as home page
  - [ ] Add Weather Dial
- Export and import old settings

##### Text Link




## Deprecated as of 2021

- Select init file place: /Dropbox/config/keysnail
- Settings
  - Prefix argument
    - [x] Use Emacs-like ...
    - Modifier + ...: C-[0-9]
- Init file Settings
  - Editor: Emacs
- Vimperator
  - [ ] Enable Vimperator like ...
- Plugins
  - Dark Theme  
  - Set Mac
  - HoK
  - Builtin command as Ext
  - Carent hint
  - Tanything
  - Keybind helper (/Dropbox/config/keysnail/keybind-helper.ks.js)
  - Option key as meta key: (/Dropbox/config/keysnail/option-as-meta.ks.js)


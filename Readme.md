# Install

* Install dependencies
```
sudo apt install i3 i3blocks rofi xbacklight
```
* Arc theme
```
sudo apt install arc-theme
```
* Useful tools
```
sudo apt install pavucontrol lxappearance
```

# Configure
## Firefox
* Font
  * install (copy ttfs to `~/.local/share/fonts`) https://github.com/supermarin/YosemiteSanFranciscoFont
* Arc-theme: https://addons.mozilla.org/en-US/firefox/addon/arc-darker-theme-we/
* Tree tabs https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/
* Remove tabs bar:
    1. set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true` in `about:config`
    2. find out profile directory in `about:support`
    3. copy the following to `$profile/chrome/userChrome.css`:
    ```
    /* hides the native tabs */
    #TabsToolbar {
    visibility: collapse;
    }/* leaves space for the window buttons */
    #nav-bar {
        margin-top: -8px;
        margin-right: 74px;
        margin-bottom: -4px;
    }
    ```
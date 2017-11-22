# Mozilla Firefox userChrome.css

Mozilla Firefox 57 'Quantum' is a big update.  Big changes for add-ons.  Visual change to the Tree Style Tab add-on.  The new Tree Style add-on works but the top tab bar still shows.  Not a big deal but it adds visual clutter. A _hide tab bar_ API is planned for later Firefox release.  Until then there are tweaks to fix the UI.

[userChrome.css](http://kb.mozillazine.org/index.php?title=UserChrome.css&printable=yes) is a text/CSS file in your Firefox Profile.  Customize elements of the Firefox user interface there.

## userChrome.css Tweaks

### Hide the top/native tabs

```css
/* hide native tabs */
#tabbrowser-tabs {
    visibility: collapse !important;
}
```

### Hide the sidebar header

This tweak removes some clutter.

```css
/* to hide the sidebar header */
#sidebar-header {
    visibility: collapse;
}
```

### Show the minimize, restore and maximize title bar buttons in Windows

```css
/* show window buttons [min, restore, max] */
#titlebar-buttonbox {
    height: 32px !important;
}
```

## File Locations

* Windows 10: C:\Users\[username]\AppData\Roaming\Mozilla\Firefox\Profiles\[profile]\chrome\userChrome.css
* Linux/Unix: ~/.mozilla/firefox.profiles/[profile]/chrome/userChrome.css

## Resources

* [Tree Style Tab by Piro - Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tree-style-tab/)
* [Tree Style Tab is a WebExtension now - ghacks.net](https://www.ghacks.net/2017/09/27/tree-style-tab-is-a-webextension-now/)
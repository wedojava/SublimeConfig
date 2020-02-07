# SublimeConfig

For Linux:

```bash
git clone https://github.com/wedojava/SublimeConfig.git ~/Git/SublimeConfig
ln -s ~/Git/SublimeConfig/sublime-snippet/ ~/.config/sublime-text-3/Packages/User/sublime-snippet
ln -s ~/Git/SublimeConfig/C.sublime-build ~/.config/sublime-text-3/Packages/User/C.sublime-build
```

For Windows:
```powershell
copy C.sublime-build %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\
mkdir %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\sublime-snippet\\
copy sublime-snippet\\* %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\sublime-snippet\\
```

# SublimeConfig

For Linux:

```bash
git clone https://github.com/wedojava/SublimeConfig.git ~/Git/SublimeConfig
ln -s ~/Git/SublimeConfig/sublime-snippet/ ~/.config/sublime-text-3/Packages/User/sublime-snippet
ln -s ~/Git/SublimeConfig/C.sublime-build ~/.config/sublime-text-3/Packages/User/C.sublime-build
sudo apt install clang-format -y
rm ~/.config/sublime-text-3/Packages/User/clang_format_custom.sublime-settings
ln -s ~/Git/SublimeConfig/clang_format_custom.sublime-settings ~/.config/sublime-text-3/Packages/User/clang_format_custom.sublime-settings
rm ~/.config/sublime-text-3/Packages/User/clang_format.sublime-settings
ln -s ~/Git/SublimeConfig/clang_format.sublime-settings ~/.config/sublime-text-3/Packages/User/clang_format.sublime-settings
```

For Windows:
```powershell
copy C.sublime-build %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\
mkdir %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\sublime-snippet\\
copy sublime-snippet\\* %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\sublime-snippet\\
copy clang_format_custom.sublime-settings %userprofile%\\scoop\\persist\\sublime-text\\Data\\Packages\\User\\
```

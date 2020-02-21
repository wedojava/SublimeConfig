# SublimeConfig

For OSX:
```bash
git clone https://github.com/wedojava/SublimeConfig.git ~/git/SublimeConfig
ln -s ~/git/SublimeConfig/sublime-snippet/ ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/sublime-snippet
ln -s ~/git/SublimeConfig/C.sublime-build ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/C.sublime-build
brew install clang-format
rm ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/clang_format_custom.sublime-settings
ln -s ~/git/SublimeConfig/clang_format_custom.sublime-settings ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/clang_format_custom.sublime-settings
rm ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/clang_format.sublime-settings
ln -s ~/git/SublimeConfig/clang_format.sublime-settings ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/clang_format.sublime-settings
```

在苹果终端输入exit命令后，竟然不退出，以下解决：
```
              ------->终端

                -------->偏好设置

                  ------->描述文件

                        -------->Shell

                          --------->单shell退出时：

                                      选择：关闭窗口
```

Sublime-text3 在苹果上 build 时过的小坑, 爱折腾的会认为是坑吧:
```
"osx":{
    "shell_cmd": "g++ '${file}' -o '${file_path}/${file_base_name}.out' && osascript -e 'tell application \"Terminal\" to activate do script \"clear&&${file_path}/${file_base_name}.out && echo \\\"Press Enter to exit.\\\"&& read line && exit && exit\"'",
}
```


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

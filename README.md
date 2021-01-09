# vscode-settings
参考https://code.visualstudio.com/docs/getstarted/settings

# 各操作系统配置文件路径
- Windows: %APPDATA%\Code\User
- macOS: $HOME/Library/Application Support/Code/User
- Linux: $HOME/.config/Code/User

The workspace settings file is located under the .vscode folder in your root folder.

# 替换配置
CODE_PATH是上面提到的路径
```
CODE_PATH="$HOME/Library/Application Support/Code/User"

SETTINGS_PATH="$CODE_PATH/settings.json"
rm -f "$SETTINGS_PATH"
ln -s "`pwd`/settings.json" "$SETTINGS_PATH"

KEYBINDINGS_PATH="$CODE_PATH/keybindings.json"
rm -f "$KEYBINDINGS_PATH"
ln -s "`pwd`/keybindings.json" "$KEYBINDINGS_PATH"
```
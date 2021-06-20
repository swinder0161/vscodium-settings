# vscodium-settings
cp keybindings.json ~/Library/Application\ Support/VSCodium/User/

cp settings.json ~/Library/Application\ Support/VSCodium/User/

# backup extension list from vscode:
code --list-extensions | tee ~/vscode-extensions.txt

# install extensions to VSCodium:
xargs -n1 codium --install-extension < ~/vscode-extensions.txt

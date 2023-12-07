### Install package dependencies:
```
sudo apt update
sudo apt install software-properties-common apt-transport-https wget -y
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```

### Install vscode:
```
sudo apt install code
```

### Change the preset editor at ubuntu:
```
sudo update-alternatives --config editor
editor
```

### Src site:
>1. https://phoenixnap.com/kb/install-vscode-ubuntu
>2. https://samwhelp.github.io/book-ubuntu-basic-skill/book/content/editor/select-editor.html

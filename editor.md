install package dependencies:
$ sudo apt update
$ sudo apt install software-properties-common apt-transport-https wget -y
$ wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
$ sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

install vscode:
$ sudo apt install code

change the preset editor at ubuntu:
$ sudo update-alternatives --config editor
$ editor

src site:
1. https://phoenixnap.com/kb/install-vscode-ubuntu
2. https://samwhelp.github.io/book-ubuntu-basic-skill/book/content/editor/select-editor.html
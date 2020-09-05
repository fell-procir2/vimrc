# Windows10

#### powershell

#### インストーラーのダウンロード。
Invoke-WebRequest https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.ps1 -OutFile installer.ps1

#### %userprofile%/.cache/deinにインストール。
./installer.ps1 ~/.cache/dein

#### _vimrcダウンロード
git clone https://github.com/fell-procir2/vimrc.git

#### %userprofile%以下に_vimrcをコピー。
cp ./_vimrc ~/

#### vim
:call dein#install()

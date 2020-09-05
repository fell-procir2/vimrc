# Windows10

#### powershell

#### インストーラーのダウンロード。
Invoke-WebRequest https://raw.githubusercontent.com/Shougo/dein.vim/master/bin/installer.ps1 -OutFile installer.ps1

#### powershellのセキュリティを一時解除。
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
-> y
#### %userprofile%/.cache/deinにインストール。
./installer.ps1 ~/.cache/dein

#### powershellのセキュリティをデフォルトに戻す。
Set-ExecutionPolicy Restricted

#### _vimrcダウンロード
git clone https://github.com/fell-procir2/vimrc.git

#### %userprofile%以下に_vimrcをコピー。
cd vimrc
cp ./_vimrc ~/

#### vim
:call dein#install()

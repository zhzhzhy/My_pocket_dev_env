# My_pocket_dev_env
A tutorial for installation of VIM-YouCompleteMe &amp; Linux-repo in Termux(Android terminal emulator)
## Installation guide
First,install Termux on your Android phone from google play store OR an apk package(No root needed)

Open your Termux
### Install Atilo
> what's Atilo?<br>
> A program to install linux on termux

Type these code
```
echo "deb [trusted=yes arch=all] https://yadominjinta.github.io/files/ termux extras" >> $PREFIX/etc/apt/sources.list
pkg update
pkg in atilo
```
More info about Atilo installation [Click here](https://github.com/YadominJinta/atilo/blob/master/README.md)

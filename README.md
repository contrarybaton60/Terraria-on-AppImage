# TerrariaOnAppImage

![Terraria running from a .AppImage file](https://codeberg.org/PeacefulWilliam/TerrariaOnAppImage/raw/branch/main/images/Terraria%20On%20AppImage.png "Terraria running from a .AppImage file")

# Preamble

Please note that I am not responsible for any legal action that could occur to you if you follow this tutorial.

This is made with the intention that you're doing this for personal use only.

This is for x86_64 computers, I don't know the outcome if your computer use a different architecture.

# Requirements

- a GOG copy of Terraria, [Buy it from GOG](https://www.gog.com/en/game/terraria)
- any GNU/Linux distribution

# Steps

## 1. Create folders

First, create an AppDir folder, for this instance we will call it Terraria.AppDir

Then, create a .desktop file, these are files will appear in your menu system if you use a program like AppImageLauncher or AM/AppMan

## 2. Drag your Terraria files to AppDir

Find your Terraria installation (by default it is `your user name/GOG Games/Terraria`) and copy the files to your AppDir folder

Rename `start.sh` to `AppRun`

## 3. Configuring the .desktop file

just add these lines and save it.
```
[Desktop Entry]
Type=Application
Name=Terraria
Icon=iconname
Categories=Game;
```
# Icons

use whatever icon you want to use and put it in your AppDir folder.

Please note that if you put your icon name in `Icon=` in your .desktop file, it should not have the file extension.

# "Compiling" the AppImage

Download the latest version of [appimagetool](https://github.com/AppImage/appimagetool/releases)

run the following command:

`ARCH=x86_64 '/pathto/appimagetool-x86_64.AppImage' '/pathto/Terraria.AppDir'`

Replace "pathto" to the path where appimagetool and Terraria.AppDir is located

now run it!

Now test if it's working, if it does, now you have a portable Terraria!
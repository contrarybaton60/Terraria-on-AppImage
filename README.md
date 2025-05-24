# TerrariaOnAppImage

![Terraria running from a .AppImage file](https://github.com/contrarybaton60/Terraria-on-AppImage/blob/main/images/Terraria%20On%20AppImage.png "Terraria running from a .AppImage file")

# Preamble

Please note that I am not responsible for any legal action that could occur to you if you follow this tutorial.

This is made with the intention that you're doing this for personal use only.

This is for x86_64 computers, I don't know the outcome if your system uses a different architecture.

# Requirements

- a GOG copy of Terraria, [Buy it from GOG](https://www.gog.com/en/game/terraria)
- any* GNU/Linux distribution

# Steps

## 1. Create files

First, create an AppDir folder. For this instance we'll name it "Terraria.AppDir".

Then create a .desktop file, this will appear in your desktop entries if using a program like [AppImageLauncher](https://github.com/TheAssassin/AppImageLauncher) or [AM](https://github.com/ivan-hc/AM).

## 2. Move Terraria files to the AppDir folder

Find your Terraria install (by default its `$HOME/GOG Games/Terraria`) and move it to your AppDir folder.

Rename `start.sh` to `AppRun`.

## 3. Configuring the .desktop file

just add these lines and save it.
```
[Desktop Entry]
Type=Application
Name=Terraria
Icon=puticonnamehere
Categories=Game;
```
# Icons

Use whatever and move it to the AppDir folder.

Note that the icon name shouldn't have the file extension in the .desktop file.

# "Compiling" the AppImage

Download the latest version of [appimagetool](https://github.com/AppImage/appimagetool/releases).

run the following command: `ARCH=x86_64 '~/pathto/appimagetool-x86_64.AppImage' '~/pathto/Terraria.AppDir'`

Replace "pathto" to the path where appimagetool and Terraria.AppDir is located, then run it.

Now test if it's working, if it does, now you have a portable Terraria!

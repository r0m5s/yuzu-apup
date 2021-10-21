# yuzu-apup

Download the latest AppImage from the Yuzu Mainline Github page.

Yuzu Mainline GitHub: https://github.com/yuzu-emu/yuzu-mainline

# Dependencies

1. AppImageLauncher
2. Possibly the normal Yuzu dependecies (need to test in other distros - only tested on arch)

# Why this script?

Basically the compiling time. I don't have a powerfull machine to always be compiling the yuzu build and since the Yuzu Team started doing Appimages I thought "Why not writing a script?".

I tried to make the script as readable possible for the people who want to see the source code and possibly change it. Always open to improve it.

# How it works

The script downloads the package to the "$HOME/Applications" which is the default folder to the AppImageLauncher and gives the permission to be executable with `chmod +x $package`.

To run it:

```bash
./update-yuzu-mainline-appimage.sh
```

After installing the AppImageLauncher will automatically create a desktop file. Just search by it like a normal application, it may takes some seconds to the AppImageLauncher to create the desktop file.

# To Do

1. Install without the need of AppImageLauncher

## License
This project is released under the MIT license.
Check out the [LICENSE](LICENSE) file for more information.

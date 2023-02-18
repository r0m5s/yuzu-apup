# yuzu-apup

Download the latest AppImage from the Yuzu Mainline Github page.

Yuzu Mainline GitHub: https://github.com/yuzu-emu/yuzu-mainline

# Dependencies

1. GNU curl
2. GNU wget

# Why this script?

Basically the compiling time. I don't have a powerful machine to always be compiling the yuzu build and since the Yuzu Team started doing Appimages I thought "Why not writing a script?".

I tried to make the script as readable possible for the people who want to see the source code and possibly change it. Always open to feedback to improve it :)

# How it works

The script automatically analyses for the most recent version of the yuzu appimage available on the official yuzu repositories, verifies if there's an existing or previous version of yuzu and downloads the new version of the application in case a new update is found. 

All the working files are in the $HOME/.local, to avoid the use of the root user, and they follow this structure:
  
  * .local/appimages/yuzu-(version).appimage - launcher
  * .local/share/applications/yuzu.desktop - Launcher desktop file
  * .local/share/icons/yuzu.svg - yuzu svg icon

# Running the Script

```bash
bash yuzu-apup
```

The script works as an updater, therefore after installing/updating simply run the application as normal.

## License
This project is released under the MIT license.
Check out the [LICENSE](LICENSE) file for more information.

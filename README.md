# yuzu-apup

Download the latest AppImage from the Yuzu Mainline Github page.

Yuzu Mainline GitHub: https://github.com/yuzu-emu/yuzu-mainline

# Dependencies

1. curl
2. wget
3. Possibly the normal Yuzu dependecies (need to test in other distros - only tested on arch)

# Why this script?

Basically the compiling time. I don't have a powerfull machine to always be compiling the yuzu build and since the Yuzu Team started doing Appimages I thought "Why not writing a script?".

I tried to make the script as readable possible for the people who want to see the source code and possibly change it. Always open to feedback to improve it :)

# How it works

All the files are created and runned in the $HOME/.local, to avoid using the root user, and they follow this structure:
  * .local/appimages - launcher
  * .local/share/applications - Launcher desktop file
  * .local/share/icons - yuzu svg icon

To run it:

```bash
./yuzu-apup
```
## License
This project is released under the MIT license.
Check out the [LICENSE](LICENSE) file for more information.

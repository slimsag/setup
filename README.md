# slimsag's good 'ol dev machine recipe

Just-bought-a-mac to having-a-coder-attack, this is slimsag's good ol' dev machine recipe.

* **Serving size**: 1
* **Prep time**: minimal
* **Bake time**: minimal
* **Features**: minimal

Ingredients: macbook of your choice (store.apple.com sells some good ones for a lot of $$$$ apparently.)

## Configure hardware

1. Sign into macOS / create user account (use credentials from note `Apple setup IDs`)
    * Use `Account name` of `slimsag` so home dir is `/Users/slimsag`
    * (I prefer to disable iCloud sync and FIleVault encryption, YMMV.)
2. Open App Store, download latest macOS version
3. Open Disk Utility, create a new APFS volume `Streaming OS` (installer will create data partition); create a second `code` partition for coding projects
4. ⌘ + Space, search for `Install macOS` and launch latest macOS installer. Install to `Streaming OS`

## Configure each OS

5. **System preferences** > **Change wallpaper** > `hexops_bg.png` (normal) or `mach_bg.png` (streaming OS)
6. Remove shit from the macOS dock, hide dock by default
7. Three-finger swipe up, create six virtual desktops
8. **Apple logo** > **About This Mac** > **More info** > change **Name** to `dev` or `streaming`
9. **System Preferences** > **Accessibility** > **Zoom** > enable digital zoom with ⌘ modifier
10. **System Preferences** > **Keyboard sensitivity** > make **Key repeat rate** as fast as possible, and **Delay until repeat** as short as possible

## Install software

11. [Firefox](https://www.mozilla.org)
    * Sign in to Mozilla (use credentials from note `Apple setup IDs`)
    * Hide bookmarks toolbar
12. [Homebrew](https://brew.sh/)
    * Run homebrew's post-install commands
13. [VSCodium](https://vscodium.com/): `brew install --cask vscodium`
    * Install `Zig Language` extension
    * DISABLE `Inlay Hints` in settings HOLY SHIT I hate those
14. [Ghostty (terminal)](https://github.com/mitchellh/ghostty)
15. [OBS Studio](https://obsproject.com/download)
    * Choose recording-only (normal OS) or streaming-only (streaming OS)
    * Choose native resolution always
16. [Stream deck Mk.II software](https://www.elgato.com/us/en/s/downloads)
17. [Discord](https://discord.com/download)
18. [zigup](https://github.com/marler8997/zigup/releases)
    * Extract, `chmod +x zigup && mkdir -p ~/.bin && mv zigup ~/.bin`
    * `echo 'export PATH="$PATH:$HOME/.bin"' >> ~/.zprofile`
19. Zig: `zigup <version>` with https://machengine.org/about/zig-version
20. Pin Firefox, Ghostty, VSCodium, OBS, Discord to dock

## You're done!

To switch between OS, hold power button longer than usual when turning on computer.

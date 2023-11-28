# slimsag's good 'ol dev setup

## Configure hardware

1. Acquire a mac (store.apple.com sells some good ones for a lot of $$$$ apparently.)
2. Sign into macOS / create user account (use credentials from note `Apple setup IDs`)
    * Use `Account name` of `slimsag` so home dir is `/Users/slimsag`
    * (I prefer to disable iCloud sync and FIleVault encryption, YMMV.)
3. Open App Store, download latest macOS version
4. Open Disk Utility, create a new APFS volume `Streaming OS` (installer will create data partition)
5. ⌘ + Space, search for `Install macOS` and launch latest macOS installer. Install to `Streaming OS`

## Configure each OS

6. **System preferences** > **Change wallpaper** > `hexops_bg.png` (normal) or `mach_bg.png` (streaming OS)
7. Remove shit from the macOS dock, hide dock by default
8. Three-finger swipe up, create six virtual desktops
9. **Apple logo** > **About This Mac** > **More info** > change **Name** to `dev` or `streaming`
10. **System Preferences** > **Accessibility** > **Zoom** > enable digital zoom with ⌘ modifier
11. **System Preferences** > **Keyboard sensitivity** > make **Key repeat rate** as fast as possible, and **Delay until repeat** as short as possible

## Install software

12. [Firefox](https://www.mozilla.org)
    * Sign in to Mozilla (use credentials from note `Apple setup IDs`)
    * Hide bookmarks toolbar
13. [Homebrew](https://brew.sh/)
    * Run homebrew's post-install commands
14. [VSCodium](https://vscodium.com/): `brew install --cask vscodium`
    * Install `Zig Language` extension
15. [Ghostty (terminal)](https://github.com/mitchellh/ghostty)
16. [OBS Studio](https://obsproject.com/download)
    * Choose recording-only (normal OS) or streaming-only (streaming OS)
    * Choose native resolution always
17. [Stream deck Mk.II software](https://www.elgato.com/us/en/s/downloads)
18. [Discord](https://discord.com/download)
19. [zigup](https://github.com/marler8997/zigup/releases)
    * Extract, `chmod +x zigup && mkdir -p ~/.bin && mv zigup ~/.bin`
    * `echo 'export PATH="$PATH:$HOME/.bin"' >> ~/.zprofile`
20. Zig: `zigup <version>` with https://machengine.org/about/zig-version
21. Pin Firefox, Ghostty, VSCodium, OBS, Discord to dock

## You're done!

To switch between OS, hold power button longer than usual when turning on computer.

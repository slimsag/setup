# slimsag's good 'ol dev setup

## Configure hardware

1. Acquire a mac (store.apple.com sells some good ones for a lot of $$$$ apparently.)
2. Sign into macOS / create user account
   3. Use credentials from note `Apple setup IDs`
   4. Use `Account name` of `slimsag` so home dir is `/Users/slimsag`
5. Open App Store, download latest macOS version
6. Open Disk Utility, create a new APFS volume `Streaming OS` (installer will create data partition)
7. ⌘ + Space, search for `Install macOS` and launch latest macOS installer. Install to `Streaming OS`

## Configure each OS

6. Three-finger swipe up, create six virtual desktops
6. **Apple logo** > **About This Mac** > **More info** > change **Name** to `dev` or `streaming`
7. Open **System Preferences** > **Accessibility** > **Zoom** > enable digital zoom with ⌘ modifier
8. Open **System Preferences** > **Keyboard sensitivity** > make **Key repeat rate** as fast as possible, and **Delay until repeat** as short as possible

## Install software

9. [Firefox](https://www.mozilla.org)
 10. Sign in to Mozilla
  * Normal OS: sign in via stephen.gutekanst
  * Streaming OS: sign in via stephen+streaming
12. [Ghostty (terminal)](https://github.com/mitchellh/ghostty)
13. [Homebrew](https://brew.sh/)
  14. Run homebrew's post-install commands
15. [VSCodium](https://vscodium.com/): `brew install --cask vscodium`
  16. Install `Zig Language` extension
14. [OBS Studio](https://obsproject.com/download)
15. [Stream deck Mk.II software](https://www.elgato.com/us/en/s/downloads)
17. [Discord](https://discord.com/download)
16. [zigup](https://github.com/marler8997/zigup/releases)
    17. Extract, `chmod +x zigup && mkdir -p ~/.bin && mv zigup ~/.bin`
    18. `echo 'export PATH="$PATH:$HOME/.bin"' >> ~/.zprofile`
16. Zig:

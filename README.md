# doppio-everforest (personal dotfiles with double bars based on everforest base16)
This is my third dotfiled rice so far. This time I focused on adding functionality to my already great setup while maintaining modularity. Direct successor to my [previous setup](https://github.com/eeelbrens/frieren-everforest).

## Previews
![2024-07-07T23_10_17,631378726+03_00](https://github.com/eeelbrens/doppio-everforest/assets/130598002/b794c0ae-f38c-4511-8ad8-853ccdd48b58)
![2024-07-07T23:08:11,427950162+03:00](https://github.com/eeelbrens/doppio-everforest/assets/130598002/0154b095-b555-41df-b8bc-74a49948daf3)
![2024-07-07T23:11:49,856793414+03:00](https://github.com/eeelbrens/doppio-everforest/assets/130598002/9fe3e13d-8734-4374-a48a-3a0b264ff7b3)


## Packages/Dependencies Used
### swaywm and co. (major UI elements)
- wm: [`sway`](https://github.com/swaywm/sway) (the base of this whole rice obv)    
> [!NOTE]
> The config files for sway depend on GNOME's GTK4.0 theming for `libadwaita` apps (i'm a GNOME departee!), as well as for user authentication within `nautilus` (via `polkit`). You may want to remove/rewrite those portions accordingly).
- main bottom bar: [`waybar`](https://github.com/Alexays/Waybar)
- lockscreen: [`swaylock`](https://github.com/swaywm/swaylock) (not shown)
- notification daemon: [`dunst`](https://github.com/dunst-project/dunst) (not shown)
- app launcher: [`wofi`](https://sr.ht/~scoopta/wofi/)
- shell: `bash` with [`ble.sh`](https://github.com/akinomyoga/ble.sh) with [`fish` like autocomplete](https://harduex.com/blog/fish-like-autosuggestions-in-bash-shell/)
- logout options: [`wlogout`](https://github.com/ArtsyMacaw/wlogout) (shown in video)

### extra dependencies required (check after your sway config copy)
- sway: `brightnessctl` `playerctl` `pamixer` `wob` (audio/brightness keybindings and progress bar), `polkit`/`polkit-gnome-authentication` (user authentication for `nautilus`), `grimshot` (for screenshots), `wf-recorder` (for screen recordings, grapped from [ugursogukpinar's gist](https://gist.github.com/ugursogukpinar/f390d9f4c829fb1b05fc74a12dd482bb)), `swayidle` (for idle settings), `swaybg` (for backgrounds, issues with this dependency missing reported on Arch), `crontab` for scheduling low battery and charging dunst alerts [Eric Murphy's dotfiles' scripts](https://github.com/ericmurphyxyz/dotfiles/tree/master/.local/bin)
- waybar: `playerctl` (for MPRIS media module)

### terminal stuff
- terminal: [`kitty`](https://github.com/kovidgoyal/kitty)
- text editor: [`nvim`](https://github.com/neovim/neovim) with [LazyVim](https://github.com/LazyVim/LazyVim) (only config files for LazyVim are included)
- fetch: [`fastfetch`](https://github.com/fastfetch-cli/fastfetch) (with custom colored logo options)

### theming stuff
- theme: [tinted-theming's base16](https://github.com/tinted-theming/home) [everforest](https://tinted-theming.github.io/base16-gallery/) (background color standardized to `#2f383e`)... here's [more info on Sainnhe's original Everforest vim theme](https://github.com/sainnhe/everforest)... for GTK4.0 (`nautilus`' theme), check [Fausto-Korpsvart's repo](https://github.com/Fausto-Korpsvart/Everforest-GTK-Theme).
- wallpaper: [this with all rights reserved](https://wall.alphacoders.com/big.php?i=1350405) (made illustration fit more into Everforest's colorscheme in Photopea using layer filters 75% Saturation + 50% Exclusion of `#2f383e`)
- firefox theming: [`csshacks`](https://mrotherguy.github.io/firefox-csshacks/) and [Adaptive Tab Bar Colour](https://github.com/easonwong-de/Adaptive-Tab-Bar-Colour).
> [!NOTE]
> The chrome folder contains my own firefox configs file for cascade. Only the cascade-colours.css file is commented out and had its color theme management to Adaptive Tab Bar Colour (background color is `#2f383e`).
- theme for websites: [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search).
- theme for YouTube: [Enhancer for YouTube](https://www.mrfdev.com/enhancer-for-youtube).
- fonts: [Jetbrains Mono](https://github.com/JetBrains/JetBrainsMono) (monospace, non-nerd variant), [Rubik](https://fonts.google.com/specimen/Rubik) (sans-serif)
- cursor: [Bibata-Modern-Classic](https://www.bibata.live/) (not shown in screenshots)

# `nvim_kit`: Daily kit for Neovim

An opinionated fork of <https://github.com/jmbuhr/quarto-nvim-kickstarter> with
some extra minimalism, intended for my own scientific writing and software
development needs. A previous, bare-bones version for Vim can be found at
<https://github.com/nhejazi/vim_edc>.

> ["Vim is a masterpiece, the gleaming precise machining tool from which so
> much of modernity was
> crafted."](https://x.com/colmmacc/status/1687861827223556096)

## Setup

Clone this repo into `~/.config/nvim/`:

```bash
git clone https://github.com/nhejazi/nvim_kit.git ~/.config/nvim
```

<!--
### Unix, Linux Installation


For displaying images in your terminal a recent version of [kitty](https://sw.kovidgoyal.net/kitty/) or [wezterm](https://wezfurlong.org/wezterm/index.html) is required
as well as the dependecies of [image.nvim](https://github.com/3rd/image.nvim) (see `./lua/plugins/ui.lua`).
Additionally, if you plan to use this through [tmux](https://github.com/tmux/tmux) make sure to have version >= 3.3a.
If you are unable to install those in your enviroment, disable the plugin by setting `enabled = false`.


Manually installing luarocks and the magick rock is no longer required, this is handled by [luarocks.nvim](https://github.com/vhyrro/luarocks.nvim).

> [!NOTE] Do this before opening nvim, otherwise `luarocks.nvim`
> might pick up the wrong luarocks version.
> If you forgot this step, you can do `:Lazy build luarocks.nvim` again manually after installation
> to fix it.



The telescope file finder uses `fzf` for fuzzy finding via the [telescope-fzf-native](https://github.com/nvim-telescope/telescope-fzf-native.nvim) extension.
It will automatically install `fzf`, but needs some requirements which are not pre-installed on Windows.
Check out the previous link for those (or comment out the extension in `./lua/plugins/ui.lua`).

Now you are good to go!
-->

## Updating

Certain updates to plugins may leave behind unused plugin data. If this
configuration produces an error on startup, try removing those first, allowing
the lazy.nvim package manager to recreate the correct plugin structure:

```bash
rm -r ~/.local/share/nvim
rm -r ~/.local/state/nvim
```

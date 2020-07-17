# Personal build of DWM
See [suckless.org](https://dwm.suckless.org "dwm.suckless.org") for the original source code.

dwm is a dynamic window manager for X. It manages windows in tiled, monocle and floating layouts. All of the layouts can be applied dynamically, optimising the environment for the application in use and the task performed.

In tiled layout windows are managed in a master and stacking area. The master area contains the window which currently needs most attention, whereas the stacking area contains all other windows. In monocle layout all windows are maximised to the screen size. In floating layout windows can be resized and moved freely. Dialog windows are always managed floating, regardless of the layout applied.

Windows are grouped by tags. Each window can be tagged with one or multiple tags. Selecting certain tags displays all windows with these tags.

Each screen contains a small status bar which displays all available tags, the layout, the number of visible windows, the title of the focused window, and the text read from the root window name property, if the screen is focused. A floating window is indicated with an empty square and a maximised floating window is indicated with a filled square before the windows title. The selected tags are indicated with a different color. The tags of the focused window are indicated with a filled square in the top left corner. The tags which are applied to one or more windows are indicated with an empty square in the top left corner.

dwm draws a small customizable border around windows to indicate the focus state.

## Patches
- [Vanitygaps](https://dwm.suckless.org/patches/vanitygaps/ "vanitygaps"): Inspired by some of the functionality of i3-gaps this patch adds (inner) gaps between client windows and (outer) gaps between windows and the screen edge in a flexible manner.
- [Swallow](https://dwm.suckless.org/patches/swallow/ "swallow"): This patch adds "window swallowing" to dwm as known from Plan 9's windowing system rio.
- [Pertag](https://dwm.suckless.org/patches/pertag/ "pertag"): More general approach to taglayouts patch. This patch keeps layout, mwfact, barpos and nmaster per tag.
- [Fibonacci](https://dwm.suckless.org/patches/fibonacci/ "fibonacci"): This patch adds two new layouts (spiral and dwindle) that arranges all windows in Fibonacci tiles: The first window uses half the screen, the second the half of the remainder, etc.
- [Systray](https://dwm.suckless.org/patches/systray/ "systray"): A simple system tray implementation. Multi-monitor is also supported. The tray follows the selected monitor.
- [Statuscmd](https://dwm.suckless.org/patches/statuscmd "statuscmd"): This patch adds the ability to execute shell commands based on the mouse button and position when clicking the status bar.
This also includes the integration with [my build](https://www.github.com/albertomosconi/dwmblocks "albertomosconi's dwmblocks") of [dwmblocks](https://github.com/torrinfail/dwmblocks "dwmblocks").
- [Xrdb](https://dwm.suckless.org/patches/xrdb "xrdb"): Allows dwm to read colors from xrdb (.Xresources) at run time. To see my dotfiles click [here](https://www.github.com/albertomosconi/dotfiles "dotfiles").

## Installation
Clone this repository in whatever folder you want to keep the source code in, then go in the cloned directory and build the package:

```bash
  git clone https://www.github.com/albertomosconi/dwm
  cd dwm
  sudo make clean install
```

## Screenshots
![busy](https://raw.githubusercontent.com/albertomosconi/dwm/master/screens/busy.jpg "busy")
![clean](https://raw.githubusercontent.com/albertomosconi/dwm/master/screens/clean.jpg "clean")

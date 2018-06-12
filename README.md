# Language Aoe2 RMS

Syntax highlighting and snippets for Age of Empires 2 random map files, with UserPatch 1.5 support.

This is very much a beta and a work in progress.

## Installation

First you should install the Atom text editor by downloading and installing it from: [https://atom.io/](https://atom.io/).
Once the editor is running use the `Ctrl-,` hotkey to open the settings tab (that is, hold `Ctrl` and press comma `,`).
The navigate to `Install` on the left sidebar and search for the `language-aoe2-rms` package.
Click the blue `Install` button to install it.
Alternatively, you may install using a command line: `apm install language-aoe2-rms`.
After installation, opening a file with the extension `.rms` will syntax highlight the file and allow you to use snippets to add code to it.

Note you can also go to the `Themes` section of the `Settings` tab to choose from different syntax highlighting color schemes.

## Snippets

Right now I have support for several snippets and plan on adding more.
To use a snippet, type in the prefix and press tab.
The snippet then expands to insert code into your file.
For example, start typing `cobj` and press `Tab`.
Then the following code is inserted
```
create_object {

}
```

A snippet may also contain several tab stops.
For example, typing `rnd` and pressing `Tab` lets you enter a value for the min number.
Then press `Tab` again to enter a value for the max number.

Right now I support the following prefixes:

| Prefix                  | Description             |
| ----------------------- | ----------------------- |
| `title` | Title for the top of your file. |
| `sections` | Adds all 7 major RMS sections. |
| `player_setup` | Adds this section |
| `land_gen` | Adds this section |
| `elevation_gen` | Adds this section |
| `cliff_gen` | Adds this section |
| `terrain_gen` | Adds this section |
| `connection_gen` | Adds this section |
| `objects_gen` | Adds this section |
| `sr` | Adds a `start_random`-`end_random` block block |
| `pc` | Adds a `percent_chance` line. |
| `cland` | Create Land |
| `cpland` | Create Player Lands |
| `cele` | Create Elevation |
| `cter` | Create Terrain |
| `cobj` | Create Object |
| `def` | Adds a `#define` directive |
| `const` | Adds a `#const` directive |
| `drs` | Adds an `#include_drs` directive |
| `aiinfo` | Adds `ai_info_map_type` |
| `rnd` | Adds `rnd(min, max)` |

## Future Plans

This is an early version I made after reading through a few tutorials on creating grammar packages, so there are bound to be bugs: please let me know about them!

I'm going to add more snippets, and perhaps keybindings for inserting things, as I play around more with rms scripting.

I'd also like to create tools for linting and autoformatting random map code.
Please let me know if you have suggestions for useful tools.

And who knows what will happen when Aoe2 DE gets released...


## smdp - A suckless command-line based markdown presentation tool

[NEW GIF COMING SOON]

### BACKGROUND
**smdp** is a fork of **[mdp](https://github.com/visit1985/mdp)**, the wonderful markdown presentation program. **smdp** is a set of modifications to my liking, namely, to make the project more suckless. Here's some notable differences:
- configuration variables were abstracted out into a config.h variable (you can now change colors and keybindings to your liking!)
- color fading and transparency was removed
- patches are encouraged (i will be providing a couple myself)

### INSTALLATION

**smdp** needs the ncursesw headers to compile. Install based on your distro, and compile using:

```
git clone https://github.com/MrPicklePinosaur/smdp.git
cd smdp
make
make install
smdp sample.md
```

### USAGE

Horizontal rulers are used as slide separator.

Supports basic markdown formating:

- line wide markup
    - headlines
    - code
    - quotes
    - unordered list

- in-line markup
    - bold text
    - underlined text
    - code

Supports headers prefixed by @ symbol.

- first two header lines are displayed as title and author
    in top and bottom bar

Review sample.md for more details.

### CONTROLS

- h, j, k, l, Arrow keys,
    Space, Enter, Backspace,
    Page Up, Page Down - next/previous slide
- Home, g - go to first slide
- End, G - go to last slide
- 1-9 - go to slide n
- r - reload input file
- q - exit

### CONFIGURATION

A `config.h` configuration file is available in `include/`, change the settings you want and recompile.
Colors, keybindings and list types are configurable as of now. Note that configuring colors only works in 8 color mode.

### CREDITS

Many kudos to the original authors and contributors of **mdp**. Once again, you can find the original project [here](https://github.com/visit1985/mdp).


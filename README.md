# Nehiyawewin-Keyboard
A Linux Keyboard layout for Plains Cree/ Nêhiyawêwin

# Example

![alt text](https://github.com/Nehiyawewin/Nehiyawewin-Keyboard/blob/main/Example.png?raw=true)

# Installation:

### Locally (for one user)

```git clone https://github.com/Nehiyawewin/Nehiyawewin-Keyboard/ && cd Nehiyawewin-Keyboard```

```mkdir -p ~/.config/xkb/symbols && cp nehiyawewin.xkb_symbols ~/.config/xkb/symbols/custom```

### Globally (for all users)

```git clone https://github.com/Nehiyawewin/Nehiyawewin-Keyboard/ && cd Nehiyawewin-Keyboard```

```cp nehiyawewin.xkb_symbols /usr/share/X11/xkb/symbols/custom```

# Usage:

If you use a typical desktop like kde, xfce, or gnome you should be able to go into your keyboard settings and select the "custom" layout

If you use a compositor / tiling window manager you will have to specify the layout in your input config, it should look something like this:

```
# Hyprland input config example

input {
    kb_layout = us, ca, custom
    kb_variant = , multix,
    kb_model =
   # kb_options = grp:alt_shift_toggle 
    kb_rules =

    numlock_by_default = true

    follow_mouse = 1

    sensitivity = 0 # -1.0 - 1.0, 0 means no modification.

    touchpad {	
        natural_scroll = false 
    }
    touchdevice {
	    enabled = true
    }
}
```

# Windows/MacOS Support:

I will not be supporting windows or macos with this project. My older archived keyboard repository should suit your needs however.

# Mod Configuration Menu

Also known as MCM. It lets you expose settings/variables in your scripts to players via a convenient menu accessible from within the game's pause menu. The settings are saved, and will persist after closing and re-opening the game.

There are various methods you can use to allow the game to interact with your settings, such as sliders, keybinds, and checkboxes. You can currently find the list on [this](https://github.com/RAX-Anomaly/Anomaly-Mod-Configuration-Menu) page, under the **How to add new sections** part, where it says **Critical Parameters**. At the time of writing, the following are available:

    "check"        	: Option, check box, either ON or OFF
    "list"         	: Option, list of strings, useful for options with too many selections
    "input"        	: Option, input box, you can type a value of your choice
    "radio_h"   	: Option, radio box, select one out of many choices. Can fit up to 8 selections (Horizental layout)
    "radio_v"   	: Option, radio box, select one out of many choices. Can fit up any number of selections (Vertical layout)
    "track"       	: Option, track bar, easy way to control numric options with min/max values (can be used only if [val] = 2)
    "key_bind"		: Option, button that registers a keypress after being clicked. (See suplimental instructions below)

This guide will demonstrate the basics of creating an MCM menu for an original mod. This consists mainly of 2 tasks: creating your mod's MCM menu, and hooking up your MCM menu options to your mod's code.

We'll begin by looking at an example mod, and then thinking about how we can configure its key variables to read in settings from a menu option.
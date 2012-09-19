sublime-text-multiple-commands
==============================

This plugin helps to run multiple commands in sublime text by one keypress

Found it at http://www.sublimetext.com/forum/viewtopic.php?f=5&t=8677

Key map is edited in user keybindings. To add multiple commands configure a key like this:

    { "keys": ["ctrl+w"],
        "command": "run_multiple_commands",
        "args": {
            "commands": [
                {"command": "find_under_expand", "context": "window"},
                {"command": "slurp_find_string", "context": "window"},
                {"command": "show_panel", "args": {"panel": "find"}, "context": "window"}
            ]
        }
    }

# SublimeText Multicommand

Plugin for sublime to run multiple commands for a keybinding

## Install

Install `Multicommand` through package control

## Usage

Open your `sublime-keymap` file from `Preferences -> Key Bindings` in Sublime Text.

Wrap the commands you want to execute within a `multicommand` section, the plugin will then execute them in order.

```json
{
  "keys": ["super+s"],
  "command": "multicommand",
  "args": {
    "commands": [
      {
        "command": "save"
      },
      {
        "command": "do_something_else"
      },
      {
        "command": "show_panel",
        "args": { "panel": "find_in_files" }
      }
    ]
  }
}
```


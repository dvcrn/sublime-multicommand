# Sublime Text Multi Commands

Plugin for sublime to run multiple commands for a keybinding

## Install

Download and put **multi_command.py** in your `/Packages/User/` directory.

You can find the directory through `Preferences -> Browse Packages` in Sublime Text. Or depending on your OS, you can allocated it at:

OSX

    ~Library/Application Support/Sublime Text 3/Packages

Windows

    C:\Users\epti-215\AppData\Roaming\Sublime Text 3\Packages

Linux

    ~/.config/sublime-text-3/Packages/

## Usage

Open your `sublime-keymap` file from `Preferences -> Key Bindings` in Sublime Text. Add multiple commands like the following examples.

### Save file & Update to evernote

In this example, when the user click "super+s", command *save* and command *save_evernote_note* will be executed.

```json
  {
    "keys": [
      "super+s"
    ],
    "command": "multi_command",
    "args": {
      "commands": [
        {
          "command": "save"
        },
        {
          "command": "save_evernote_note",
          "context": [
            {
              "key": "evernote_note"
            }
          ]
        }
      ]
    }
  }
```

## Credit

For Sublime Text Multi Commands, credit gose to its original author, **Nilium**.
For [Sublime Evernote](https://github.com/bordaigorl/sublime-evernote), credit goes to its contributors.

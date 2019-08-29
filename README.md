# Sublime Text Multi Commands

Plugin for sublime to run multiple commands for a keybinding

## Install

## Usage

Open your `sublime-keymap` file from `Preferences -> Key Bindings` in Sublime Text. 

In this example, when the user click "super+s", command *save* and command *save_evernote_note* will be executed.

```json
  {
    "keys": [
      "super+s"
    ],
    "command": "multicommand",
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

## License

MIT

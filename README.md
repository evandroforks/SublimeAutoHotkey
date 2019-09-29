# SublimeAutoHotkey - Syntax Package for Sublime Text 2/3
AutoHotkey AHK language package for SublimeText including syntax highlighting, comments toggling, auto-completions, build system definitions, commands for ahkrun, ahkcompile, ahkrunpiped.


## Installation

### By Package Control

1. Download & Install `Sublime Text 3` (https://www.sublimetext.com/3)
1. Go to the menu `Tools -> Install Package Control`, then,
   wait few seconds until the `Package Control` installation finishes
1. Go to the menu `Preferences -> Package Control`
1. Type `Package Control Add Channel` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, input the following address and press <kbd>Enter</kbd>
   ```
   https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
   ```
1. Now, go again to the menu `Preferences -> Package Control`
1. This time type `Package Control Install Package` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, search for `AutoHotkey` and press <kbd>Enter</kbd>

See also:
1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


## Key Bindings
If you have the default Sublime keybindings intact, then:
* <kbd>Ctrl+B</kbd> will run the current file (with AutoHotkey.exe)
* <kbd>Ctrl+Shift+B</kbd> will compile the current file (with Ahk2Exe.exe)

## Advanced Configuration
For the build system and ahkrun, ahkrunpiped, and ahkcompile commands, if you have a non-default installation then you will need to set your specific path to AutoHotkey.exe and Ahk2Exe.exe in a file named AutoHotkey.sublime-settings in your User folder. You can access these settings file from the Menu `Preferences > Package Settings > AutoHotkey`. You should make a copy of `AutoHotkey Settings - Default` at `AutoHotkey Settings - User` and modify there since then any settings defined in your User folder will take precedence and the package can still update itself without overwriting your custom settings.

## ahkrunpiped
The ahkrunpiped command will allow you to run your code as a piped text string to AutoHotkey (this allows you to run snippets of code without having to save them to a file):
* If text is selected - ahkrunpiped will pipe and run the selected text only.
* If no text is selected - ahkrunpiped will pipe and run the entire contents of the current document.

## Goto-documentation Integration
Instructions on how to configure goto-documentation plugin for AutoHotkey (F1 Hotkey will take you to documentation for word under cursor)
* http://www.autohotkey.com/board/topic/46447-sublime-text-editor-very-nice/page-3#entry540187

## Credits
* S0und: http://www.autohotkey.com/board/topic/46447-sublime-text-editor-very-nice/page-2#entry529723
* Misc: http://www.sublimetext.com/forum/viewtopic.php?f=2&t=4008
* Misc: http://www.autohotkey.com/board/topic/44924-yatmb4ahk-yet-another-textmate-bundle-for-ahk/
* ahkrunpiped, Coco: https://gist.github.com/cocobelgica/6296475
* ahkrunpiped, greycode: https://gist.github.com/grey-code/4728413
* ahkrunpiped, Lexikos: http://www.autohotkey.com/board/topic/23575-how-to-run-dynamic-script-through-a-pipe/

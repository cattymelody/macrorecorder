# MacroRecorder
Script for LuaMacros that let you record macros without programming required.

Download link:
https://github.com/mrsimb/macrorecorder/archive/master.zip

GitHub:
https://github.com/mrsimb/macrorecorder

LuaMacros:
https://github.com/me2d13/luamacros

## Before you start
This script is only for use with additional keypad/keyboard.

After initial start of the script, all your keyboards will try to work as usual,
but will lag in some way. That is due to LuaMacros limitations.

When you're done with recording macros for your keypad, go to "SETTINGS SECTION"
and change use("all") to use("your_keypad_id").

ID is shown in log form of LuaMacros window every time you press any key.
Default record hotkey is INSERT (key code 45).

## How to use
1. Press and hold your hotkey combination ("ctrl c", for example)
2. Press INSERT (do it quickly!) and release all keys
3. Type your macro
4. Press INSERT again
5. Done. Now every time you press "ctrl c" script will reproduce recorded key sequence.

## Removing macro:
1. Press and hold your hotkey combination
2. Press INSERT and release all keys
3. Press INSERT again, without typing any sequence

## Changing record hotkey
1. Look for correct key code in "KEY NAMES TABLE"
2. Change macroHotkey code in "SETTINGS SECTION"

## Using embed functions as macros
1. Record your macro
2. Open "macros.lua" and find your hotkey
3. Write a function instead of key sequence
4. Example: ['^(c'] = function() print('embed function!') end

## Known issues
- Rocording only works with English layout (due to LuaMacros bug).
- Recording shift+(abc), and sending it results Abc, not ABC (due to LuaMacros bug).

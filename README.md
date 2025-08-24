# VSCode set up for competitive programming

## Getting started
1. Install `build-essential` & `valgrind`:
```bash
sudo apt install build-essential
sudo apt install valgrind
```
2. Add to your VSCode project the file `.vscode/tasks.json` and replace the macro `JP` with yours.
3. Add the following keybindings to your `keybindings.json`. 
```json
[
     {
        "key": "Ctrl+0",
        "command": "workbench.action.tasks.runTask",
        "args": "compile",
        "when": "editorTextFocus"
    },
    {
        "key": "Ctrl+9",
        "command": "workbench.action.tasks.runTask", 
        "args": "valgrind-run",
        "when": "editorTextFocus"
    },
    {
        "key": "Ctrl+1",
        "command": "workbench.action.tasks.runTask", 
        "args": "valgrind-run-1",
        "when": "editorTextFocus"
    },
    {
        "key": "Ctrl+2",
        "command": "workbench.action.tasks.runTask", 
        "args": "valgrind-run-2",
        "when": "editorTextFocus"
    },
    {
        "key": "Ctrl+3",
        "command": "workbench.action.tasks.runTask", 
        "args": "valgrind-run-3",
        "when": "editorTextFocus"
    }
]
```
You can access this file with `Ctrl+Shift+P` and typing `Preferences: Open Keyboard Shortcuts (JSON)`.

## Shortcuts 
The supported shortcuts are:
* `Ctrl+0`: compiles the file `./sol.cpp`.
* `Ctrl+9`: run the file `./sol` using valgrind with the specified input file.
* `Ctrl+1`: run the file `./sol` using valgrind with the `1.in` file as input.
* `Ctrl+2`: run the file `./sol` using valgrind with the `2.in` file as input.
* `Ctrl+2`: run the file `./sol` using valgrind with the `3.in` file as input.

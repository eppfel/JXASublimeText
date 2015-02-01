# JXASublimeText
This package makes it easier to use your favorite editor Sublime Text to program with JavaScript for Automation. This works just on Mac OSX Yosemite (10.10). For now I created the build system.

## Build System
Run and Build commands for Scripts, Script Bundles and Applets. Choose 'JXA' from `Tools > Build Systems`.

The standard `Build` command creates an executable and in Apple Script Editor editable script file (.scpt).

The `Run` command executes the script directly in ST.
In the command palette are more variants to build:
- `Build: App`: Build an executable application (.app)
- `Build: Script Bundle`: Build an executable Script Bundle (.scptd)

The Build System takes a vanilla JavaScript file and runs the shell command `osascript -l Javascript [file_name]` or `osacompile -l JavaScript -o [file_name].scpt [file_name]`. Look the `osacompile` manual for more options.

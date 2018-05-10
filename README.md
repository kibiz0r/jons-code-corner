# jons-code-corner

## Setup

### Git

1. Make a Github account
1. Fork this repository
1. [Install Github for Windows](https://desktop.github.com/)
1. File -> Clone repository and select your jons-code-corner repo

### MinGW

1. [Download MinGW](https://cytranet.dl.sourceforge.net/project/mingw/Installer/mingw-get-setup.exe)
1. Install MinGW with C++ development packages
![MinGW packages](/.README/mingw.png)
1. Start menu -> Edit the system environment variables -> Environment Variables...
1. Double-click User Variable `Path`
1. New: `C:\MinGW\bin`

### Visual Studio Code

1. [Install Visual Studio Code](https://code.visualstudio.com/)
1. [Install C++ Extensions](vscode:extension/ms-vscode.cpptools)

## Build

1. Tasks -> Run Build Task

## Run

1. Debug -> Start Without Debugging

You should see output in the Debug Console (View -> Debug Console if it's not visible)

## Modifying

Pretty much everything comes down to `tasks.json` and `launch.json`. VSCode has good documentation on both. You'll also need to know how to invoke `g++` in general. Right now, it's just compiling everything in one go with no intermediate object files, using `g++` directly. In the future, maybe we'll switch to use `make`.
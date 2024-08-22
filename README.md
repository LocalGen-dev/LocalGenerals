<div align="center">
  <h1>Local Generals.io</h1>
  <a href="http://github.com/SZXC-WG/LocalGen-new/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/SZXC-WG/LocalGen-new.svg" /></a>
  <a href="http://github.com/SZXC-WG/LocalGen-new/releases"><img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/SZXC-WG/LocalGen-new.svg" /></a>
  <a href="http://github.com/SZXC-WG/LocalGen-new/LICENSE.md"><img alt="License" src="https://img.shields.io/github/license/SZXC-WG/LocalGen-new.svg" /></a>
  <a href="http://github.com/SZXC-WG/LocalGen-new/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/SZXC-WG/LocalGen-new.svg?style=social" /></a>
  <h2><font color="red">branch <code>v5-EGE</code></font></h2>
</div>

Welcome to Local Generals.io, branch `v5-EGE`.

This branch contains the source code and (some) documentation of LocalGen Version 5.

GUI here is built with [EGE Graphics library](http://xege.org).

To contribute to this project, please create an issue or create a pull request. **Thank you for supporting LocalGen.**

## Build instructions

LocalGen v5 is built using [CMake](https://cmake.org/). Make sure it's installed on your system before building.

### Building through command lines

First, check your [MinGW-w64](https://mingw-w64.org/) installation and make sure it's on PATH.

Assuming you have cloned the project and switched to its directory in the terminal, initialize with the following command:

```bash
mkdir build
cd build
cmake .. -G "MinGW Makefiles"
```

> [!TIP]
> Initializing more than once is not necessary, unless `CMakeLists.txt` is changed.

Finally, build the executable `LGen.exe`:

```bash
cmake --build . --config Release
```

> [!IMPORTANT] 
>
> **For devs**
> Please test in debug mode after making changes to the source code:
>
> ```bash
> cmake --build .
> ```


### If you use VS Code...

We have the [CMake Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools) extension as an alternative for building the project.

`settings.json` is already configured to build with MinGW Makefiles. Please manually select the `GCC` compiler kit and set variant to `Release` for compilation.

## Known issues

- Web mode may not work when using speed 1. Try 2 or higher.

# Pong Game

A classic Pong game made with C++ and [raylib 4.5.0](https://github.com/raysan5/raylib/releases/tag/4.5.0). Control the right paddle and play against a computer-controlled opponent.

## Controls

- **Up Arrow**: move the player paddle up.
- **Down Arrow**: move the player paddle down.
- **Close the window**: quit the game.

## Requirements

- Windows
- [raylib 4.5.0](https://github.com/raysan5/raylib/releases/tag/4.5.0)
- [w64devkit](https://github.com/skeeto/w64devkit/releases) with GNU Make and a C++ compiler

The build command below assumes w64devkit is installed at `C:/raylib/w64devkit` and raylib at `C:/raylib/raylib`. Change those paths if your setup differs.

## Build

Run this command from the project directory in PowerShell:

```powershell
C:/raylib/w64devkit/bin/make.exe RAYLIB_PATH=C:/raylib/raylib PROJECT_NAME=main OBJS=main.cpp
```

This creates `main.exe` in the project directory.

## Run

```powershell
./main.exe
```

If Windows reports that a compiler DLL is missing, run the game from a w64devkit terminal or add `C:/raylib/w64devkit/bin` to your `PATH`.

## Project files

- `main.cpp` - game source code.
- `Makefile` - build configuration.

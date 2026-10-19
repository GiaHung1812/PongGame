# Pong Game

A simple two-player-style Pong game built with C++ and [raylib](https://www.raylib.com/). You control the right paddle, while the computer controls the left paddle. Score by getting the ball past the other paddle.

## Controls

- **Up Arrow**: move your paddle up.
- **Down Arrow**: move your paddle down.
- **Close the game window**: quit.

## Requirements

- A C++ compiler with C++14 support.
- [raylib 4.5.0](https://github.com/raysan5/raylib/releases/tag/4.5.0), including its headers and library.
- GNU Make. On Windows, the included Makefile is configured for raylib's **w64devkit** toolchain.

## Build and run on Windows

The included VS Code build tasks expect w64devkit at `C:/raylib/w64devkit/bin` and raylib at `C:/raylib/raylib`. If raylib is installed elsewhere, change `RAYLIB_PATH` to its location.

From the project directory, build with:

```powershell
C:/raylib/w64devkit/bin/make.exe RAYLIB_PATH=C:/raylib/raylib PROJECT_NAME=main OBJS=main.cpp
```

Run the game with:

```powershell
./main.exe
```

If you are using the included VS Code setup, you can also choose **Terminal > Run Build Task** and select a build task.

## Project files

- `main.cpp` - game source code.
- `Makefile` - build configuration for raylib.

The generated executable and compiler DLLs are build/runtime files and are excluded from Git. Build the game locally using the instructions above.

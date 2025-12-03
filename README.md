> [!WARNING]
> While I haven't ran into any issues, this project is **not** thread safe due to a lack of read locking in `world.zig`! A planned fix by using [`std.Thread.RwLock`](https://ziglang.org/documentation/master/std/#std.Thread.RwLock) and adding the according locks. For now, please be aware of this issue.

> [!NOTE]  
> This repository **will be archived** after necessary fixes have been made (and possibly added [emscripten](https://emscripten.org/) compilation target support). Sokol is great, but I wanted more control and features without worrying about shader compatibility, and have moved on to a new project.
# block_game.zig
[![build](https://github.com/spencrc/block_game.zig/actions/workflows/zig.yml/badge.svg)](https://github.com/spencrc/block_game.zig/actions/workflows/zig.yml)
## Supported Platforms
This project only **runs only on MacOS and Windows**. Linux is **not supported** and **will** crash at runtime!
## Building & Running
Using Zig 0.15.2, you can build the project
```
zig build
```
This will produce an executable. You can run the executable itself, or build and run the project with
```
zig build run
```

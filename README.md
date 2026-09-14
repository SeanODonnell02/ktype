# ktype
an adaptive terminal typing trainer written in c11, Inspired from keybr.com. ktype generates pseudo words from the letters that you're the weakest at, tracks per-key speed and accuracy, and unlocks new letters as you improve.

## Features 
 - Per-keystroke timing and error tracking for every key
 - Adaptive lesson generation based on your slowest keys 
 - Progressive alphabet unlocking based on a speed and accuracy threshold 
 - Persistent profile across sessions 
 - Zero dependencies beyond a POSIX libc

## Requirements
 - A POSIX system (macOS, Linux, WSL2) with a VT100-compatible terminal
 - A C11 compiler and CMake 3.20+

## Build
```sh
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build
./build/ktype
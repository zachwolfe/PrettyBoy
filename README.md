# PrettyBoy
PrettyBoy is a work-in-progress Game Boy emulator written in Dusk, a work-in-progress programming language.

# Current status
Currently, my goal is to get the bootrom running, and transferring control to a game (update: this is basically done, but there are a few bugs to iron out). The next step will be getting graphics working well enough to render the scrolling Nintendo logo on boot. Then, I will want to get Tetris working, and then I will move on to more complicated games. The immediate problem is that while Dusk is envisioned as a compiled language, only an interpreter is implemented so far. Because of this (and because the interpreter is not very well optimized), performance of running the gameboy bootrom is currently very bad.

# How to run
1. Probably just don't, actually. Dusk is still extremely rough around the edges. Also, though Dusk has almost as much support for Linux and macOS as it does Windows, PrettyBoy directly depends on some Win32 APIs, so only Windows is supported for the time being.
1. If you insist, clone the [Dusk "compiler"](https://github.com/dusklang/dusk)
1. From the root of the Dusk repo, with [Rust](https://www.rust-lang.org/learn/get-started) installed, install Dusk by running `cargo install --path dusk`
1. Clone PrettyBoy, and to the root of the repository, copy legally-obtained copies of the DMG bootrom and Tetris as `bios.bin` and `tetris.bin`, respectively
1. run `dusk main.dusk`
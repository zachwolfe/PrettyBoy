# PrettyBoy
PrettyBoy is a work-in-progress Game Boy emulator written in Dusk, an unreleased programming language.

# Current status
Currently, my goal is to get the bootrom running, and transferring control to a game. The next step will be getting Tetris working, and then I will move on to more complicated games. The immediate problem is that while Dusk is envisioned as a compiled language, only an interpreter is implemented so far. Because of this, performance of running the gameboy bootrom is currently sitting at around 90 ms / frame. That will need to be improved. But it used to be about 50 times worse than that. Progress!

# How to run
- Step 1: steal the Dusk source code from my private repository
- Step 2: turn yourself into the police
- Step 3: from prison, install Dusk
- Step 4: navigate to the PrettyBoy root folder and install your legally-obtained copies of the DMG bootrom and Tetris as bios.bin and tetris.bin, respectively.
- Step 5: run `dusk main.dusk`
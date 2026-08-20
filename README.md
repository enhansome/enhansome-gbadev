# Awesome Game Boy Advance development with stars

A curated list of development resources for Game Boy Advance.

Contribute adding resources or providing feedback through Pull Requests, Issues or joining us on [Discord](https://discord.io/gbadev). You can find a web version of this list [here](https://gbadev.net).

## Table of Contents

* [Introduction](#introduction)
  * [Community](#community)
* [Documentation](#documentation)
  * [Tutorials](#tutorials)
  * [Articles](#articles)
* [Software Development](#software-development)
  * [Compilers](#compilers)
  * [Toolkits](#toolkits)
  * [Libraries](#libraries)
  * [Emulators](#emulators)
* [Emulator Development](#emulator-development)
  * [Testing](#testing)
* [Homebrews](#homebrews)
  * [Jams](#jams)
* [Miscellanea](#miscellanea)
  * [Dumping the GBA BIOS](#dumping-the-gba-bios)
  * [Reverse engineering](#reverse-engineering)
  * [Historical links](#historical-links)

***

# Introduction

* [Technical introduction to the GBA](https://copetti.org/projects/consoles/game-boy-advance)

## Community

* [GBAdev Forum](https://forum.gbadev.net) - Our new hub for announcements and long-form discussion. It's a good place to ask questions and share progress on your projects.
* [GBAdev Discord / IRC](https://gbadev.net/chat.html) - This is where everyone hangs out to chat nowadays. Come say hi!

### Other places

* [GBAdev.org](https://gbadev.org) - The longstanding homepage of the scene. Still updated with news and releases (but the forums have been broken for a while).
* [GBAtemp](https://gbatemp.net/categories/nintendo-gba-discussions.32/) - The site carries the GBA name, but nowadays the console is relegated to the backbenches. It's a good place to talk about gaming and hardware though.

# Documentation

* [GBATEK](https://problemkaputt.de/gbatek.htm) - Programming specs for the GBA and NDS hardware
* [CowBite Virtual Hardware Specifications](https://www.cs.rit.edu/~tjh8300/CowBite/CowBiteSpec.htm) - Older GBA hardware documentation
* [The Audio Advance](http://belogic.com/gba/) - Audio hardware documentation and basic test ROMs

## Tutorials

* [Tonc](https://gbadev.net/tonc/) - The new, revamped version of the GBA programming tutorial. The original version is [here](https://www.coranac.com/tonc/text/toc.htm).
* [Compile C++ for GBA in under an hour](https://www.youtube.com/watch?v=EMeie_gSgDU) - Cinemint's video for getting started with C++/Butano
* [Sound on the Gameboy Advance](https://stuij.github.io/deku-sound-tutorial/) - How to write your own sound mixer / MOD music player
* [Larold's Retro Gameyard - Game Boy Advance Tutorials](https://laroldsretrogameyard.com/category/tutorials/gba/) - Learn how to make GBA games using the Butano Game Engine. Each part of the engine will have own individual tutorial with example source code.

## Articles

* [Gameboy Advance Resource Management](https://www.gamedeveloper.com/programming/gameboy-advance-resource-management) - Allocation techniques for the GBA's various memory regions
* [Managing Sprite Cel VRAM on the Game Boy Advance](https://pineight.com/gba/managing-sprite-vram.txt) - Analysis of the VRAM streaming approach for animated sprites
* [Using Beepbox for GBA Music Composition](https://rentry.org/beepbox-gba-music)

# Software Development

## Compilers

* [TinyGo](https://github.com/tinygo-org/tinygo) ⭐ 17,657 | 🐛 564 | 🌐 Go | 📅 2026-08-19 - An alternative Go compiler for embedded systems, that supports GBA compilation
* [gba-toolchain](https://github.com/felixjones/gba-toolchain) ⭐ 139 | 🐛 4 | 🌐 CMake | 📅 2026-04-01 - GNU Arm Embedded Toolchain based alternative to devkitARM.
* [gvasm](https://github.com/velipso/gvasm) ⭐ 70 | 🐛 10 | 🌐 TypeScript | 📅 2024-12-07 - Stand-alone assembler and disassembler (WIP) designed specifically for GBA homebrew
* [devkitARM](https://devkitpro.org) - C/C++ cross-compiler toolchain, which includes libgba, libtonc, maxmod, and various tools and example projects.

## Toolkits

* [Butano](https://github.com/GValiente/butano) ⭐ 1,744 | 🐛 0 | 🌐 C++ | 📅 2026-08-06 - Modern C++ high level engine for the GBA.
* [rust-console](https://github.com/rust-console/gba) ⭐ 723 | 🐛 7 | 🌐 Rust | 📅 2026-08-13 - GBA programming in Rust, plus tutorial.
* [ZigGBA](https://github.com/wendigojaeger/ZigGBA) ⭐ 386 | 🐛 7 | 🌐 Zig | 📅 2025-07-19 - WIP SDK for creating GBA games using Zig (Inspired by Tonc).
* [natu](https://github.com/exelotl/natu) ⭐ 249 | 🐛 0 | 🌐 Nim | 📅 2025-02-15 - GBA programming in Nim (provides wrapper around libtonc, maxmod and more).
* [BPCore Engine](https://github.com/evanbowman/BPCore-Engine) ⭐ 208 | 🐛 13 | 🌐 C++ | 📅 2024-06-28 - Create GBA applications with the Lua programming language
* [gbsenpai](https://github.com/asiekierka/gbsenpai) ⚠️ Archived - GB Studio player GBA port with some enhancements.
* [gba-modern](https://github.com/JoaoBaptMG/gba-modern) ⭐ 88 | 🐛 2 | 🌐 C++ | 📅 2023-06-26 - Write GBA games using modern C++.
* [rath](https://github.com/stuij/rath) ⭐ 41 | 🐛 0 | 🌐 C | 📅 2022-12-12 - Forth programming environment for the Game Boy Advance
* [meson-gba](https://github.com/LunarLambda/meson-gba) ⚠️ Archived - Meson-based GBA toolkit with support for many different libraries and tools.
* [GBA Dlang](https://github.com/redthing1/gba_dlang) ⭐ 17 | 🐛 0 | 🌐 D | 📅 2022-02-21 - WIP SDK for GBA development using D, using LLVM toolchain. provides fully functional TONC, GBFS, Maxmod.
* [ada-gba-dev](https://github.com/98devin/ada-gba-dev) ⭐ 12 | 🐛 3 | 🌐 Ada | 📅 2023-07-24 - A build system, libraries, and tools for producing programs for the Game Boy Advance using the Ada programming language.
* [dusk](https://github.com/redthing1/dusk) - Simple, lightweight, intuitive framework for GBA game development
* [sdk-seven](https://github.com/sdk-seven) - Modern runtime and tooling, and libraries for GBA development. Works with meson-gba or standalone.
* [agb](https://agbrs.dev) - Rust high level framework for the GBA with a build system, asset importing, tracker player and graphics abstractions.

## Libraries

* [GBT Player](https://github.com/AntonioND/gbt-player) ⭐ 304 | 🐛 0 | 🌐 C | 📅 2026-01-25 - Music library that uses the DMG sound channels (close to 0% CPU usage).
* [gba-link-connection](https://github.com/afska/gba-link-connection) ⭐ 293 | 🐛 0 | 🌐 C++ | 📅 2026-08-01: A set of C++ libraries to interact with the Serial Port (Link Cable, Wireless Adapter, GPIO, SPI)
* [agbabi](https://github.com/felixjones/agbabi) ⭐ 79 | 🐛 3 | 🌐 C | 📅 2024-05-10 - Drop-in application binary interface library (context switching, division, irq, memcpy, sine).
* [Krawall](https://github.com/sebknzl/krawall) ⭐ 69 | 🐛 2 | 🌐 C | 📅 2014-10-01 - Music and sound library (supports .xm, .s3m)
* [Apex Audio System](https://github.com/stuij/apex-audio-system) ⭐ 52 | 🐛 2 | 🌐 C | 📅 2023-10-20 - Music and sound library (supports .mod only, but *very* good performance)
* [HeartLib](https://github.com/Sterophonick/HeartLib) ⚠️ Archived - Comprehensive C library inspired by the classic HAMLib.
* [gba-hpp](https://github.com/felixjones/gba-hpp) ⭐ 29 | 🐛 0 | 🌐 C++ | 📅 2024-04-20 - C++20 header-only library for GBA development.
* [GBAdv](https://github.com/sverx/GBAdv) ⭐ 29 | 🐛 0 | 🌐 C | 📅 2022-12-15 - High level utilities on top of libgba.
* [Pimpmobile](https://github.com/kusma/pimpmobile) ⭐ 27 | 🐛 0 | 🌐 C | 📅 2022-04-07 - Music library (supports .mod, .xm)
* [libseven](https://github.com/sdk-seven/libseven) ⚠️ Archived - Modern, from-scratch replacement for libgba and libtonc.
* [gbaLib](https://github.com/MnlPhlp/gbaLib) ⭐ 9 | 🐛 0 | 🌐 Go | 📅 2021-10-29 - Library for programming the GBA with TinyGo
* [Maxmod](https://maxmod.devkitpro.org) - Music and sound library (supports .mod, .xm, .s3m, .it)
* [posprintf](http://www.danposluns.com/gbadev/posprintf/index.html) - An `sprintf` routine written in Thumb assembler.
* [GBFS](https://pineight.com/gba/#gbfs) - Practical filesystem

## Emulators

* [NanoBoyAdvance](https://github.com/nba-emu/NanoBoyAdvance) ⚠️ Archived - GBA emulator with high accuracy, especially in timing and CPU emulation. Does not have debugging features.
* [SkyEmu](https://github.com/skylersaleh/SkyEmu) ⭐ 1,239 | 🐛 255 | 🌐 C | 📅 2026-06-26 - GB/GBA/NDS Emulator with built in debuggers, REST API for scripting, and high accuracy.
* [MiSTer FPGA implementation](https://github.com/MiSTer-devel/GBA_MiSTer) ⭐ 176 | 🐛 20 | 🌐 VHDL | 📅 2026-07-22 - Needs [MiSTer](https://github.com/MiSTer-devel/Main_MiSTer/wiki) ⭐ 3,273 | 🐛 132 | 🌐 C++ | 📅 2026-08-17 setup to run.
* [mGBA](https://mgba.io) - Actively developed GBA emulator. Runs on a bunch of platforms. Text debugger through GDB stub.
* [No$gba](https://problemkaputt.de/gba.htm) - Venerable GBA emulator. Windows only, but runs well under Wine. Not very actively maintained but still gets updates now and then. Sports graphical debugger.
* [Mesen](https://mesen.ca/) - Multi-system emulator with high GBA accuracy. It provides great built-in GUI tools such as a debugger, a profiler and an event viewer.

# Emulator Development

## Testing

* [240p-test-mini](https://github.com/pinobatch/240p-test-mini) ⭐ 290 | 🐛 8 | 🌐 Assembly | 📅 2026-07-09 - video signal tests
* [GBA Suite](https://github.com/jsmolka/gba-suite) ⭐ 134 | 🐛 0 | 🌐 Assembly | 📅 2025-04-19
* [mGBA test suite](https://github.com/mgba-emu/suite) ⭐ 102 | 🐛 9 | 🌐 C | 📅 2026-07-09
* [NBA hardware tests](https://github.com/nba-emu/hw-test) ⚠️ Archived

# Homebrews

* [OpenLara](https://github.com/XProger/OpenLara) ⭐ 5,060 | 🐛 167 | 🌐 C | 📅 2026-07-26 - Classic Tomb Raider open-source engine
* [Celeste Classic](https://github.com/JeffRuLz/Celeste-Classic-GBA) ⭐ 393 | 🐛 2 | 🌐 C | 📅 2025-04-09 - 2019 port of Pico8 version of Celeste.
* [GBADoom](https://github.com/doomhack/GBADoom) ⭐ 294 | 🐛 24 | 🌐 C | 📅 2025-09-29 - 2019/2020 GBA port of prBoom version of Doom.
* [BlindJump](https://github.com/evanbowman/blind-jump-portable) ⭐ 231 | 🐛 4 | 🌐 C++ | 📅 2023-07-07 - Adventure game, developed in 2020. Implementation of link-cable multiplayer, fully digital audio.
* [Goodboy Advance](https://github.com/exelotl/goodboy-advance) ⭐ 71 | 🐛 0 | 🌐 C | 📅 2023-01-01 - Made in 2018, and has a nice bit of information on how it's made.
* [Tigermoth](https://github.com/pmprog/TigermothGBA) ⭐ 17 | 🐛 0 | 🌐 C | 📅 2021-06-19 - Bullet hell game, developed for the GBAJam 2021
* [Duster](https://github.com/redthing1/duster) - A sleek strategy board game for the gba

# Jams

* [GBA Jam 2021](https://itch.io/jam/gbajam21/entries)
* [GBA Winter Jam '21](https://itch.io/jam/gba-winter-jam-2021/entries)
* [GBA Jam 2022](https://itch.io/jam/gbajam22/entries)
* [GBA Winter Jam '23](https://itch.io/jam/gba-winter-jam-23)
* [GBA Microjam '23](https://gbadev.itch.io/gba-microjam-23)
* [GBA Jam 2024](https://itch.io/jam/gbajam24/entries)

# Miscellanea

* [GBA bare metal code](https://github.com/PeterLemon/GBA) ⭐ 144 | 🐛 1 | 🌐 Assembly | 📅 2021-05-27 - Various experiments by Krom, such as video playback and 3D, written in ARM Assembly
* [gba\_bios](https://github.com/PikalaxALT/gba_bios) ⭐ 47 | 🐛 1 | 🌐 C++ | 📅 2025-08-09 - WIP disassembly of the Game Boy Advance BIOS
* [Usenti](https://github.com/gb-archive/usenti) ⭐ 15 | 🐛 0 | 📅 2024-07-28 - Simple bitmap editor for paletted images aimed at GBA development.
* [dkarm\_gba\_docker](https://github.com/redthing1/dkarm_gba_docker) - A Docker image that includes DevkitARM and other GBA SDK tools, packaged together to allow a consistent toolchain configuration and reproducibility in builds. Also can be helpful in ensuring a consistent build environment for continuous integration.
* [RGB55 colour picker](https://orangegb.com/BGR555/) - Tool for picking colours in the BGR555 colour format the GBA uses.

## Dumping the GBA BIOS

* [Software interrupt $1F / MidiKey2Freq](https://web.archive.org/web/20230321185310/https://gist.github.com/modwizcode/b4afc78ea74fb453be3bcaf3d3bc8adc), canonical method
* [Cracking the GBA BIOS](https://mgba.io/2017/06/30/cracking-gba-bios/) by endrift
* [Dumping the GBA BIOS](https://web.archive.org/web/20210616201436/https://gist.github.com/MerryMage/797c523724e2dc02ada86a1cfadea3ee), another method by MerryMage

## Reverse engineering

* [Pokemon Ruby](https://github.com/pret/pokeruby) ⭐ 983 | 🐛 32 | 🌐 C | 📅 2026-04-09 - C programming language annotation of a Pokemon Ruby disassembly
* [Reverse Engineering a GameBoy Advance Game](https://medium.com/@bruno.macabeus/reverse-engineering-a-gameboy-advance-game-introduction-ec185bd8e02) - A series of detailed posts and talks about developing a [level editor](https://github.com/macabeus/klo-gba.js) ⭐ 166 | 🐛 4 | 🌐 JavaScript | 📅 2023-10-01 for *Klonoa: Empire of Dreams*

## Historical links

* [HEL](http://www.console-dev.de/project/hel-library-for-gba/) - GBA C library built on top of HAM (a classic SDK from back in the day)
* [Headspin's Guide](https://web.archive.org/web/20230130121359/http://members.iinet.net.au/~freeaxs/gbacomp/) to Compression, Files Systems, Screen Effects and MOD Players for the Gameboy Advance

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-20._

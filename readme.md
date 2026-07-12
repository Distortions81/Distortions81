<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=header&text=Carl+Otto&fontSize=48&fontColor=ffffff&desc=Distortions81&descAlignY=68&descSize=18" alt="Carl Otto Header"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?lines=Systems+Programming+%7C+Infrastructure+Tooling;Go+Development%2C+Automation%2C+and+Applied+Engineering&center=true&width=700&height=35" alt="Typing SVG" />
</p>

## About Me

I work across software, electronics, and data, with a focus on systems programming, game development, automation, and infrastructure-oriented tooling. My projects often combine implementation with measurement, using benchmarks, visualizations, and prototypes to make trade-offs explicit.  

I approach projects iteratively: build, measure, refine, and document. Some repositories are production-ready tools, while others are focused experiments used to validate a design or architectural approach.  

I value efficiency and leverage through automation, clear interfaces, and practical tooling that reduces friction between an idea and a working system.  

In practice, that means building systems, observing how they behave, and refining them until they are reliable, understandable, and useful.

## Project Snapshots
Small thumbnails from projects where visuals help show the work at a glance.

<table>
  <tr>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/GD-DOOM">
        <img src="assets/project-thumbnails/gd-doom.png" alt="GD-DOOM gameplay thumbnail" width="150"><br>
        <sub>GD-DOOM</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/GD-WOLF">
        <img src="assets/project-thumbnails/gd-wolf.png" alt="GD-WOLF gameplay thumbnail" width="150"><br>
        <sub>GD-WOLF</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/M45-goPool">
        <img src="assets/project-thumbnails/m45-gopool.png" alt="M45-goPool dashboard thumbnail" width="150"><br>
        <sub>M45-goPool</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/M45-Core-Firmware">
        <img src="assets/project-thumbnails/m45-core-firmware.png" alt="M45-Core-Firmware stats thumbnail" width="150"><br>
        <sub>M45-Core-Firmware</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/goThoom">
        <img src="assets/project-thumbnails/gothoom.png" alt="goThoom client thumbnail" width="150"><br>
        <sub>goThoom</sub>
      </a>
    </td>
  </tr>
  <tr>
    <td align="center" width="20%">
      <a href="https://github.com/M45-Science/ChatWire">
        <img src="assets/project-thumbnails/chatwire.png" alt="ChatWire logo thumbnail" width="150"><br>
        <sub>ChatWire</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/ONI-SeedView">
        <img src="assets/project-thumbnails/oni-seedview.png" alt="ONI-SeedView map thumbnail" width="150"><br>
        <sub>ONI-SeedView</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/EUI">
        <img src="assets/project-thumbnails/eui.png" alt="EUI demo thumbnail" width="150"><br>
        <sub>EUI</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/PixelPirates">
        <img src="assets/project-thumbnails/pixelpirates.png" alt="PixelPirates gameplay thumbnail" width="150"><br>
        <sub>PixelPirates</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/ImpSynth">
        <img src="assets/project-thumbnails/impsynth.png" alt="ImpSynth logo thumbnail" width="150"><br>
        <sub>ImpSynth</sub>
      </a>
    </td>
  </tr>
</table>

## Featured Projects
A selection of repositories that reflect the range of systems, tools, and experiments I work on, ordered roughly by complexity, scope, and technical depth.

Repository metadata was refreshed from GitHub on July 12, 2026. Lines of code are approximate tracked source/text lines, excluding binary assets, vendored dependencies, and build output.

### [GD-DOOM](https://github.com/Distortions81/GD-DOOM)
**Language:** Go | **Complexity:** Very High

Go-based Doom engine with two presentation targets: a `Faithful` mode that stays close to vanilla Doom behavior, and a `Source Port` mode that enables 32-bit RGBA rendering, sub-tic interpolation for camera/things/weapons, OPL-style and SoundFont MIDI music backends, enhanced automap, and other quality-of-life upgrades. Loads original WAD data directly; supports IWAD/PWAD combinations, save/load, demo recording and playback, and runs in-browser via WebAssembly.

[Play in browser](https://m45sci.xyz/u/dist/GD-DOOM/)
*Lines of Code:* ~173k

**Highlights:**
- Dual render modes: faithful colormap-based shading vs. distance-lit source-port path with independent GPU sky
- Sub-tic interpolation for camera yaw, thing positions, weapon sprites, and animated textures/flats
- Two music backends: `impsynth` (OPL3-style, hardware feel) and `meltysynth` (SoundFont General MIDI)
- Full game flow: episode/skill menus, save/load, demo playback/recording, in-game IWAD picker
- Runs on Linux, Windows, macOS (Intel + Apple Silicon), and in-browser via WebAssembly

### [GD-WOLF](https://github.com/Distortions81/GD-WOLF)
**Language:** Go | **Complexity:** High

Go/Ebiten Wolfenstein 3D port focused on gameplay parity with native and WebAssembly targets. It includes software raycast rendering, HUD/status presentation, save-slot previews, persistent settings, spatial audio, and optional modern render modes.

*Lines of Code:* ~29.3k

**Highlights:**
- Wolfenstein 3D-style raycast renderer, status bar, pause/options menus, elevators, and level transitions
- Native and browser builds, with embedded shareware fallback data for the WebAssembly target
- Save slot previews with thumbnails plus browser save persistence on wasm
- Selectable `DOS`, `HQ`, and `ULTRA` render modes with configurable input, audio, and VSync settings
- Enemy parity work supported by fuzz, harness, and soak-test tooling

### [goThoom](https://github.com/Distortions81/goThoom)
**Language:** Go | **Complexity:** High

Modern open-source client for the classic Clan Lord MMORPG. Cross-platform desktop application built on Ebiten with OpenGL, DirectX, and Metal rendering, plus plugin support.

*Lines of Code:* ~60.3k

**Highlights:**
- Cross-platform desktop client built on Ebiten with OpenGL, DirectX, and Metal backends
- Plugin system powered by Yaegi for runtime extensibility and experimentation
- Quality-of-life upgrades including text-to-speech and automatic asset fetching
- Performance-focused rendering improvements, including de-dithering for legacy graphics

### [M45-goPool](https://github.com/Distortions81/M45-goPool)
**Language:** Go | **Complexity:** High

Standalone Bitcoin mining pool designed to pair with Bitcoin Core over JSON-RPC and ZMQ, serve Stratum v1 miners over plain TCP or TLS, expose an HTTPS-first status UI and JSON API, manage TLS certificates automatically, and provide thorough configuration, operations, and testing documentation.

*Lines of Code:* ~61.5k (including tests)

**Highlights:**
- Deep Bitcoin Core integration via JSON-RPC longpoll + ZMQ block feed for Stratum v1 mining
- Production-minded pool controls: rate limiting, invalid-share bans, reconnect churn mitigation, and TLS support
- Configurable coinbase split handling for fees, donations, and miner payouts
- Strong ops/testing ergonomics with install scripts, profiling helpers, and detailed `operations.md`, `performance.md`, and `TESTING.md`

### [M45-Core-Firmware](https://github.com/Distortions81/M45-Core-Firmware)
**Language:** C/C++ | **Complexity:** High

ESP32-WROOM-32 Bitcoin mining firmware built with ESP-IDF. It combines Stratum mining, hardware SHA candidate loops, OLED/LCD status surfaces, and local web setup, stats, and settings pages for a compact standalone miner controller.

*Lines of Code:* ~17k

**Highlights:**
- ESP-IDF build, environment-check, flash, serial-monitor, and benchmark helper scripts
- Stratum mining flow covering protocol parsing, target handling, share queues, self-checks, and task management
- OLED display UI plus optional ideaspark LCD target and local web status/settings/setup pages
- Current `v0.0.5` build snapshot: 725 KiB OLED app, 957 KiB LCD app, and about 620 kH/s average mining speed
- Hardware-focused implementation for ESP32-WROOM-32 constraints

### [M45-Gamma-Firmware](https://github.com/Distortions81/M45-Gamma-Firmware)
**Language:** C | **Complexity:** High

Experimental firmware for Bitaxe Gamma 602 miners. It boots at stock BM1370 ASIC settings, exposes a local web dashboard, and adds browser-based controls for Wi-Fi, pool failover, fan behavior, safety limits, overclocking, OTA updates, and recovery through a Web Serial flasher.

[Open the Web Flasher](https://distortions81.github.io/M45-Gamma-Firmware/)
*Lines of Code:* ~23.6k

**Highlights:**
- Targets ESP32-S3 Gamma 602 hardware with BM1370 ASIC, TPS546 PMBus regulator, EMC2101 fan controller, and SSD1306 OLED
- First-install and recovery flow through a browser Web Serial flasher, plus OTA package generation
- Live dashboard for hashrate, ASIC state, temperatures, fan, power, best diff, block alerts, and pool status
- Configurable safety limits, stock-default boot behavior, optional unrestricted test mode, and hardware self-test on firmware changes
- Native M45 JSON endpoints plus ESP-Miner-compatible JSON routes for external tooling

### [ChatWire](https://github.com/M45-Science/ChatWire)
**Language:** Go | **Complexity:** High

A long-running bridge between Discord and Factorio servers that supports server management and moderation workflows.
Part of the [M45-Science](https://github.com/M45-Science) GitHub organization ([website](https://m45sci.xyz/)).
Active since 2017.

*Lines of Code:* ~24.1k

**Highlights:**
- Long-running Discord-to-Factorio bridge built with [DiscordGo](https://github.com/bwmarrin/discordgo)
- Server orchestration and process control for managing multiple game instances
- Custom game/mod update workflows using the Factorio [Download API](https://wiki.factorio.com/Download_API) and [Mod Portal API](https://wiki.factorio.com/Mod_portal_API)
- Real-time operations tooling with WebSockets, HTTP APIs, and live logging/diagnostics

### [GoMUD2](https://github.com/Distortions81/GoMUD2)
**Language:** Go | **Complexity:** Medium-High

A full MUD server written in Go, featuring an online creation (OLC) world editor, telnet support with TLS, 256-color ANSI rendering, and a structured command/permission system.

*Lines of Code:* ~13k

**Highlights:**
- Telnet server with optional TLS for encrypted connections
- In-game OLC world editor for building and modifying areas at runtime
- 256-color ANSI terminal rendering with theme support
- Permission and role system for player/builder/admin workflows

### [ONI-SeedView](https://github.com/Distortions81/ONI-SeedView)
**Language:** Go | **Complexity:** Medium

WebAssembly map seed viewer for [Oxygen Not Included](https://www.klei.com/games/oxygen-not-included) built with [Ebiten](https://ebitengine.org/). It retrieves [seed data](https://mapsnotincluded.org/) and renders an interactive map with detailed biome and object information.

[Try it here](https://m45sci.xyz/u/dist/oni-view/view.html?coord=SNDST-A-1-0-0-0)
*Lines of Code:* ~6.2k

**Highlights:**
- Parses and visualizes ONI seed data in-browser using Go + WebAssembly
- Interactive map exploration with detailed overlays and adjustable UI scaling
- Export support for high-resolution printable maps
- Mobile-friendly touch controls and alternate viewer integration on [MapsNotIncluded.org](https://mapsnotincluded.org/map-explorer/SNDST-A-1-0-0-0)

### [EUI](https://github.com/Distortions81/EUI)
**Language:** Go | **Complexity:** Medium

Minimal retained-mode UI library for Ebiten, using vector-drawn windows, flows, widgets, themes, and scaling logic for game and tool interfaces.

[Live demo](https://m45sci.xyz/u/dist/eui/)
*Lines of Code:* ~12.1k

**Highlights:**
- Draggable and resizable windows, overlay items, portal windows, and flow layouts
- JSON-backed palettes and styles with runtime theme switching and auto-reload support
- UI scaling, cached widget rendering, tree dumps, debug overlays, and touch support
- Common controls including buttons, sliders, checkboxes, radios, dropdowns, hidden inputs, image labels, and tooltips
- Runs anywhere Ebiten runs, including desktop, web, and mobile targets

### Factorio [SoftMod](https://github.com/M45-Science/SoftMod) (for [M45-Science](https://github.com/M45-Science))
**Language:** Lua | **Complexity:** Medium-High

Scenario scripting for M45-Science Factorio servers, focused on softmod-style server administration and gameplay support.

*Lines of Code:* ~10k

**Highlights:**
- Scenario-based server scripting with no client-side mod download required
- Dynamic GUI systems and permission-based commands for moderation/admin workflows
- Player-driven moderation features (including vote-banish) and action logging
- Localization support across multiple languages with live server usage in production

### [PixelPirates](https://github.com/Distortions81/PixelPirates)
**Language:** Go | **Complexity:** Medium-Low

Retro sailing and exploration prototype centered on rendering experiments and gameplay feel.

[Play online](https://m45sci.xyz/u/dist/pixelpirate)
*Lines of Code:* ~6.9k
[Blog post about this project](https://carlotto81.wixsite.com/m45-science/post/solo-game-developer-adventures)

**Highlights:**
- Custom real-time music synthesizer
- Perlin noise-driven procedural sky generation
- Runs well in-browser via WebAssembly
- Can import sprite sheets from [Aseprite](https://www.aseprite.org/)

### [ImpSynth](https://github.com/Distortions81/ImpSynth)
**Language:** Go | **Complexity:** Medium

Compact OPL3-style FM synthesis library in Go focused on the practical DMX/Doom-era register subset: 2-operator voices, envelopes, feedback, waveforms, stereo panning, and direct OPL-style register writes.

*Lines of Code:* ~6.8k

**Highlights:**
- Focused FM synth implementation tuned around the classic Doom/DMX-style OPL workflow
- Simple register-driven API with stereo `int16` PCM generation
- Includes an example renderer that converts melody CSV + patch JSON inputs into `.wav` output
- Zero-allocation PCM benchmark noted in the repo docs for real-time-friendly synthesis work

### [GoBeep86](https://github.com/Distortions81/GoBeep86)
**Language:** Go | **Complexity:** Medium-Low

PC speaker audio emulator for Go programs that need retro beeps, simple music, or sound effects with physical speaker and case coloration instead of a clean square wave.

*Lines of Code:* ~1.7k

**Highlights:**
- Simulates clean, paper-cone speaker, and piezo-style output variants
- Adds steel-case resonance and ringing for old-machine speaker character
- Supports streaming through an `io.Reader` source or offline rendering to stereo `int16` PCM
- Can interleave effect and music tone sequences to emulate a single physical speaker
- Accepts PIT-divisor tone streams and PCM music re-driven through a simulated 1-bit speaker path

### [go-g726](https://github.com/Distortions81/go-g726)
**Language:** Go | **Complexity:** Medium-Low

G.726 ADPCM codec library for mono 8 kHz audio, with explicit 2, 3, 4, and 5 bits-per-sample modes and streaming-safe encoder/decoder state handling.

*Lines of Code:* ~2k

**Highlights:**
- Stateful `Encoder` and `Decoder` types for continuous audio streams
- One-shot helpers for simple buffer-to-buffer conversions
- Size helpers and framing validation for each supported bit depth
- Reset support for independent packets or clips
- Recent work focused on streaming state correctness and packed-group behavior for non-4-bit modes

### [numfmt](https://github.com/Distortions81/numfmt)
**Language:** Go | **Complexity:** Medium-Low

Compact numeric encoding library for large positive values that trades exactness for predictable error bounds, reducing the size of telemetry, snapshots, and other high-volume numeric payloads.

*Lines of Code:* ~1.7k

**Highlights:**
- Encodes values into compact `8`/`16`/`32` bit integer codes using tunable exponent and mantissa sizing
- Supports constrained ranges and automatic exponent sizing for domain-specific quantization
- Includes a binary payload format for packing whole numeric slices with self-describing codec metadata
- Ships with a small JavaScript codec plus generated quantization-guide docs for cross-language use and evaluation

### [goXA](https://github.com/Distortions81/goXA)
**Language:** Go | **Complexity:** Medium-Low

Custom archiving utility built around a compact archive format.

*Lines of Code:* ~5.8k

**Highlights:**
- Custom archive structure
- Checksums, many compression types
- Preserve file permissions, mod times
- Offers forward error correction
- Threaded compression options

### [goMMO](https://github.com/Distortions81/goMMO)
**Language:** Go | **Complexity:** Medium-Low

Client-side MMO prototype that explores small-world simulation, WebSocket communication, and low-bandwidth networking techniques.

*Lines of Code:* ~5.1k

**Highlights:**
- WebSocket networking
- Custom low-bandwidth binary networking protocol
- Linear interpolation for smooth movement/frame pacing at low update rates (8 Hz base)
- Hashmap-backed chunk system for efficient world state management
- Serialized game-data caching to reduce CPU load in busy areas

### [FactBanSync](https://github.com/M45-Science/FactBanSync)
**Language:** Go | **Complexity:** Medium

Synchronizes ban lists across multiple Factorio servers, with a CLI merge tool and lightweight web API for centralized management.

[Web Interface](https://m45sci.xyz:8443/)
*Lines of Code:* ~2.2k

**Highlights:**
- Data synchronization
- CLI tool design
- JSON processing
- Lightweight web server

### [FactorioServerBrowser](https://github.com/M45-Science/FactorioServerBrowser)
**Language:** Go | **Complexity:** Medium-Low

Minimal Factorio server browser with a web interface. Polls servers on a schedule, caches results, and serves a simple index page.

[Live Demo](https://factorio.go-game.net/)
*Lines of Code:* ~2k

**Highlights:**
- RESTful HTTP handling
- Server polling and caching
- Front-end/back-end integration
- Uses [matchmaking](https://wiki.factorio.com/Matchmaking_API) API

### [DownloadProxy](https://github.com/M45-Science/DownloadProxy)
**Language:** Go | **Complexity:** Medium-Low

Local HTTP caching proxy for Factorio server environments, designed to reduce repeated upstream downloads for server automation running behind ChatWire on a trusted LAN.

*Lines of Code:* ~2.2k

**Highlights:**
- Restricts access to localhost and an explicit Factorio-focused upstream allowlist
- Caches release downloads, checksum files, mod downloads, and selected API responses on disk
- Preserves useful upstream metadata such as content type, ETag, last-modified, and disposition headers
- Throttles cache misses before contacting upstream servers
- Keeps the design intentionally narrow instead of acting as a general-purpose open proxy

### [GoRecoverBlurText](https://github.com/Distortions81/GoRecoverBlurText)
**Language:** Go | **Complexity:** Medium
Experimental tool that attempts to recover blurred or pixelated text through brute-force comparison.
*Lines of Code:* ~384

### [golang-frac](https://github.com/Distortions81/golang-frac)
**Language:** Go | **Complexity:** Medium
Mandelbrot fractal renderer for high-detail image and video frame generation.

*Lines of Code:* ~225

**Highlights:**
- Multi-threaded Mandelbrot rendering
- High-resolution frame/image generation
- CLI-controlled zoom and render parameters

### [goMarketMadness](https://github.com/Distortions81/goMarketMadness)
**Language:** Go | **Complexity:** Medium
A tribute to a childhood type-in economic simulation, reimplemented in Go.

[Play it here](https://m45sci.xyz/u/dist/otto/marketmadness/)
*Lines of Code:* ~2.3k

**Highlights:**
- Simulates TUI of TI-99/4a
- Game loop and economic modeling (Brownian noise)
- Event-driven simulation

## Curated Project Map
Repository metadata was checked with GitHub CLI on July 12, 2026. Public repositories are linked. Private repositories are intentionally listed without links.

### Most Intriguing First
| Project | Visibility | Area | Why it stands out |
| --- | --- | --- | --- |
| [GD-DOOM](https://github.com/Distortions81/GD-DOOM) | Public | Game engine / WebAssembly | Full Doom engine work in Go with faithful and enhanced presentation modes, original WAD loading, save/demo support, native builds, and browser play. |
| Encore-4A | Private | FPGA / retrocomputing | Verilog hardware work at the intersection of soft CPUs, classic systems, and low-level implementation. |
| [M45-goPool](https://github.com/Distortions81/M45-goPool) | Public | Bitcoin infrastructure | Standalone mining pool with Bitcoin Core integration, Stratum serving, TLS, operational tooling, and production-minded failure controls. |
| [M45-Gamma-Firmware](https://github.com/Distortions81/M45-Gamma-Firmware) | Public | Embedded firmware | Firmware for Bitaxe Gamma 602 miners with browser flashing, OTA packaging, safety controls, and hardware-facing diagnostics. |
| [M45-Core-Firmware](https://github.com/Distortions81/M45-Core-Firmware) | Public | Embedded firmware | ESP32 mining controller firmware combining Stratum, hardware SHA loops, display UI, web setup, stats, and settings. |
| [goThoom](https://github.com/Distortions81/goThoom) | Public | Desktop client | Modern Clan Lord client in Go/Ebiten with cross-platform rendering, plugin support, asset handling, and accessibility-oriented features. |
| [GD-WOLF](https://github.com/Distortions81/GD-WOLF) | Public | Game engine / WebAssembly | Wolfenstein 3D-style engine work with software raycasting, save previews, browser persistence, and selectable render modes. |
| [ChatWire](https://github.com/M45-Science/ChatWire) | Public | Game server operations | Long-running Discord and Factorio bridge with moderation, server orchestration, HTTP APIs, WebSockets, and live ops tooling. |
| Facility38 | Private | Simulation | Massively parallel game simulation proof-of-concept focused on scale and systems behavior. |
| TMX9999-FPGA | Private | FPGA / CPU design | Verilog CPU work targeting the TMS9900 instruction set on Tang Nano hardware. |
| [ONI-SeedView](https://github.com/Distortions81/ONI-SeedView) | Public | Visualization / WebAssembly | Interactive Oxygen Not Included seed viewer using Go, Ebiten, map overlays, exports, and mobile-friendly controls. |
| [EUI](https://github.com/Distortions81/EUI) | Public | UI toolkit | Retained-mode UI library for Ebiten with windows, flows, widgets, themes, scaling, debug overlays, and touch support. |

### Hardware, Infrastructure, and Ops
| Project | Visibility | Language | Notes |
| --- | --- | --- | --- |
| [M45-goPool](https://github.com/Distortions81/M45-goPool) | Public | Go | Bitcoin pool software with JSON-RPC/ZMQ integration, Stratum, TLS, metrics, and hardening controls. |
| [M45-Gamma-Firmware](https://github.com/Distortions81/M45-Gamma-Firmware) | Public | C | Gamma 602 firmware, Web Serial flashing, OTA flow, dashboard, and ASIC safety controls. |
| [M45-Core-Firmware](https://github.com/Distortions81/M45-Core-Firmware) | Public | C++ | ESP32-WROOM-32 Bitcoin mining firmware with display and local web UI. |
| Encore-4A | Private | Verilog | FPGA retrocomputing work. |
| LM32-FPGA | Private | Verilog | FPGA soft CPU work using LM32 tooling. |
| TMX9999-FPGA | Private | Verilog | FPGA CPU compatible with the TMS9900 instruction set. |
| ProtonSync | Private | Go | Systems automation / sync tooling. |
| [DaVinci-Resolve-Container](https://github.com/Distortions81/DaVinci-Resolve-Container) | Public | Shell | Containerized DaVinci Resolve workflow for Ubuntu 24.04. |
| [Canon-Webcam-Linux](https://github.com/Distortions81/Canon-Webcam-Linux) | Public | Shell | Linux webcam support tooling. |
| [PCB-Frame](https://github.com/Distortions81/PCB-Frame) | Public | OpenSCAD | Parametric PCB display stand. |

### Games, Clients, and Interactive Tools
| Project | Visibility | Language | Notes |
| --- | --- | --- | --- |
| [GD-DOOM](https://github.com/Distortions81/GD-DOOM) | Public | Go | Doom engine, browser target, save/load, demos, and enhanced rendering/audio paths. |
| [GD-WOLF](https://github.com/Distortions81/GD-WOLF) | Public | Go | Wolfenstein 3D-style engine with native and browser builds. |
| [goThoom](https://github.com/Distortions81/goThoom) | Public | Go | Cross-platform Clan Lord client with plugin support. |
| [ONI-SeedView](https://github.com/Distortions81/ONI-SeedView) | Public | Go | Interactive ONI seed viewer and map export tool. |
| [PixelPirates](https://github.com/Distortions81/PixelPirates) | Public | Go | Retro sailing prototype with procedural sky and custom music synthesis. |
| [goMMO](https://github.com/Distortions81/goMMO) / [goMMOServ](https://github.com/Distortions81/goMMOServ) | Public | Go | Small-world MMO networking prototype and server. |
| [GoMUD2](https://github.com/Distortions81/GoMUD2) | Public | Go | MUD server with telnet, TLS, ANSI rendering, OLC, and roles. |
| LumenClay | Private | Go | MUD project work. |
| Void-Colony | Private | Go | Game prototype work. |
| Shellworld | Private | Go | Web-based terminal game prototype. |
| [goMarketMadness](https://github.com/Distortions81/goMarketMadness) / [Market-Madness-TI99](https://github.com/Distortions81/Market-Madness-TI99) | Public | Go / BASIC | Reimplementation and source preservation for a childhood type-in economic game. |

### Libraries, Media, and Experiments
| Project | Visibility | Language | Notes |
| --- | --- | --- | --- |
| [EUI](https://github.com/Distortions81/EUI) | Public | Go | Retained-mode UI toolkit for Ebiten projects. |
| [ImpSynth](https://github.com/Distortions81/ImpSynth) | Public | Go | OPL-style FM synthesis library focused on Doom/DMX-era register workflows. |
| [GoBeep86](https://github.com/Distortions81/GoBeep86) | Public | Go | PC speaker emulator with physical speaker and case coloration. |
| [go-g726](https://github.com/Distortions81/go-g726) | Public | Go | Streaming-safe G.726 ADPCM codec library. |
| [numfmt](https://github.com/Distortions81/numfmt) | Public | Go | Compact numeric encoding with tunable precision and small payload formats. |
| [goXA](https://github.com/Distortions81/goXA) | Public | Go | Lightweight archive format with compression, checksums, permissions, and FEC options. |
| [Acoustic-Space-Rendering](https://github.com/Distortions81/Acoustic-Space-Rendering) | Public | Go | OpenCL pressure simulation experiment. |
| [OpenCLFrac](https://github.com/Distortions81/OpenCLFrac) / [golang-frac](https://github.com/Distortions81/golang-frac) | Public | Go | Fractal rendering experiments across CPU and OpenCL paths. |
| [GoRecoverBlurText](https://github.com/Distortions81/GoRecoverBlurText) | Public | Go | Demonstrates brute-force recovery of blurred or pixelated text. |
| QR-Img | Private | Go | Image/QR experiment. |
| GFEC | Private | Go | Experimental forward error correction encoding. |
| Network-Sim | Private | Go | Network simulation work. |

### M45-Science Operations and Factorio Tooling
| Project | Visibility | Language | Notes |
| --- | --- | --- | --- |
| [ChatWire](https://github.com/M45-Science/ChatWire) | Public | Go | Discord-to-Factorio bridge, server manager, APIs, and live diagnostics. |
| [SoftMod](https://github.com/M45-Science/SoftMod) | Public | Lua | Scenario scripting for M45-Science Factorio servers. |
| [FactorioServerBrowser](https://github.com/M45-Science/FactorioServerBrowser) | Public | Go | Cached web-accessible Factorio server browser. |
| [DownloadProxy](https://github.com/M45-Science/DownloadProxy) | Public | Go | Narrow caching proxy for Factorio releases, mods, and API responses. |
| [FactBanSync](https://github.com/M45-Science/FactBanSync) | Public | Go | Ban-list synchronization and merge tooling. |
| [FactorioCommunityList](https://github.com/M45-Science/FactorioCommunityList) | Public | Data | Public directory of Factorio communities with public ban lists. |
| [RelayClient](https://github.com/M45-Science/RelayClient) / [RelayUpdater](https://github.com/M45-Science/RelayUpdater) | Public | Go | Network relay client and update deployment tooling. |
| [RoleBot](https://github.com/M45-Science/RoleBot) / [HelpBot](https://github.com/M45-Science/HelpBot) | Public | Go | Discord support automation. |
| [QuickBanCombine](https://github.com/M45-Science/QuickBanCombine), [MapArchiveCleaner](https://github.com/M45-Science/MapArchiveCleaner), [MapSettings](https://github.com/M45-Science/MapSettings) | Public | Go / Data | Small operational tools and data used around Factorio server administration. |
| FactMapGen | Private | Go | Factorio map generation tooling. |
| FactModDatDecode | Private | Go | Factorio mod data decoding work. |

### Smaller Public Utilities
| Project | Language | Notes |
| --- | --- | --- |
| [SolarLightCalc](https://github.com/Distortions81/SolarLightCalc) | HTML | Solar garden light solar/battery calculator. |
| [IrPowerOn](https://github.com/Distortions81/IrPowerOn) | C++ | Arduino IR power-on helper for TVs. |
| [goClanLordImgExport](https://github.com/Distortions81/goClanLordImgExport) / [goClanLordSndExport](https://github.com/Distortions81/goClanLordSndExport) | Go / C | Clan Lord asset extraction tools. |
| [goPixelChat](https://github.com/Distortions81/goPixelChat) | Go | Twitch chat pixel canvas experiment. |
| [goRaycast2](https://github.com/Distortions81/goRaycast2) | Go | Old-school raycasting experiment. |
| [goSnake](https://github.com/Distortions81/goSnake) / [goSnakeServ](https://github.com/Distortions81/goSnakeServ) | Go | Small multiplayer snake client/server. |
| [Collatz](https://github.com/Distortions81/Collatz), [SeqPrimeGo](https://github.com/Distortions81/SeqPrimeGo), [InterferencePattern](https://github.com/Distortions81/InterferencePattern) | Go | Math and simulation experiments. |
| [goWordSearch](https://github.com/Distortions81/goWordSearch), [goCardinal](https://github.com/Distortions81/goCardinal), [goKillComments](https://github.com/Distortions81/goKillComments) | Go | Small text, number, and source-processing utilities. |

_Thank you for visiting._

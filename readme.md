# Carl Otto · Distortions81

**Systems programming, embedded firmware, FPGA hardware, game engines, and infrastructure.**

I work across software, electronics, and data, usually with Go at the center.
My projects range from desktop and browser game engines to microcontroller
firmware, FPGA systems, and services used in day-to-day operations.

Most of my current work lives in private repositories. The overview below
covers that work as well as public projects you can explore, run, or play.

I approach projects iteratively: build, measure, refine, and document.
Benchmarks, visualizations, hardware experiments, and operational feedback help
me understand where a design works and where it needs another pass. Some
projects become maintained tools; others remain focused experiments in an
architecture, protocol, or piece of hardware.

## Private projects & ongoing engineering

Private work makes up a large part of my portfolio, especially in FPGA and
retrocomputing systems, embedded telemetry, infrastructure, and simulation.
These projects are described here without repository links.

### FPGA & retrocomputing

| Project | Focus |
| --- | --- |
| **Encore-4A** | A passive TI-99/4A side-port snooper for the Tang Nano 20K. It reconstructs VDP and PSG state to produce HDMI video and audio, with emulator-fed replay support for development and comparison. |
| **RetraceGPU** | Quake-oriented FPGA graphics system for the Tang Console Neo, splitting game and geometry work on an Andes CPU from FPGA rasterization, depth, textures, lighting, and display output. Active renderer and memory-system development. |
| **Project-Retrace** | A modern retrocomputing platform built around the Tang Console 138K. It combines an in-tree MC68000-compatible soft CPU, 720p HDMI text and packed framebuffers, flash-loaded applications, and BL616 USB input. The goal is an understandable system with modern conveniences. |
| **FocusTerm** | A Tang Nano 20K hardware terminal with a shared 80×24 display pipeline, multiple FPGA video targets, and an optional ESP32 companion for SSH and SPI connectivity. |
| **VectorFPGA** | A 3D vector interpretation of Doom, with a framebufferless Tang Mega 138K renderer. One atomic UART-fed vector list drives either 720p HDMI or analog X/Y output for an oscilloscope. |
| **TMX9999-FPGA** | TMS9900-compatible soft CPU and SoC work, including HDMI text and graphics, a UART monitor, flash-loaded firmware, and compiled BASIC bring-up. |
| **TangSHA256 / TangScrypt** | FPGA hashing experiments: a standalone Verilog SHA-256d scanner with a Go host, and a SpinalHDL Scrypt ROMix accelerator with on-chip scratchpads. SHA-256d results are simulation- and timing-tested; hardware validation remains separate. |
| **LM32-FPGA** | An attempt to build a fast, binary-compatible LatticeMico32 implementation, wrapped in a small SoC with RAM, UART, LED I/O, HDMI, flash storage, and benchmark tooling. |

### UI toolkit

| Project | Focus |
| --- | --- |
| **EUI** | Retained-mode Ebiten UI library with windows, flows, widgets, themes, scaling, debug overlays, and touch support. |

### Infrastructure, embedded systems & simulation

| Project | Focus |
| --- | --- |
| **BTCFlux** | A low-latency Bitcoin block-relay overlay with regional peers, compact-block transport, forward error correction, and a gateway to unmodified Bitcoin Core. Core retains block validation responsibility. |
| **Scout T1** | ESP32/MCP9808 temperature telemetry over ESP-NOW, with relays, an ESP32-S3 BLE gateway, and browser trends and history. Firmware and UI development are ahead of full hardware validation. |
| **BatteryMesh** | ESP32/ESP-NOW store-and-forward battery telemetry across sensor, relay, gateway, and bridge roles. Includes BLE and self-hosted web dashboards, current measurement, and capacity tracking. |
| **Facility38** | A factory-building game and massively parallel simulation proof of concept, exploring production, logistics, resource flows, and interacting systems at scale. |
| **PoolCensus, goBitaxeRemote & related Bitcoin tooling** | Private tools for pool measurement, miner management, data inspection, and operations, alongside experiments such as ScriptSigSearch, stratum-binary-batch, and bitgraph. |
| **FactModDatDecode & relayServer** | Supporting Factorio tooling for mod-data decoding and server infrastructure. |
| **EvoLife** | Go ecosystem simulation with inherited traits, sensory motor networks, mutation, feeding guilds, and inspectable lineage and population history. Browser and native Ebitengine views share checkpoint-based experiments. |

## Selected public projects

These are useful entry points into the parts of my work available publicly.

| Project | What it does |
| --- | --- |
| [GD-DOOM](https://github.com/Distortions81/GD-DOOM) | A Doom engine and source port written in Go for desktop and browser. GPU drawing preserves the software-rendered appearance, with classic and modern presentation, WAD loading, saves, demos, and FM, SoundFont, or PC speaker audio. [Play](https://m45sci.xyz/u/dist/GD-DOOM/) |
| [GD-WOLF](https://github.com/Distortions81/GD-WOLF) | Wolfenstein 3D-style engine in Go with software raycasting, save previews, browser persistence, spatial audio, and selectable render modes. [Play](https://m45sci.xyz/u/dist/GD-WOLF/) |
| [goThoom](https://github.com/Distortions81/goThoom) | A modern Windows, macOS, and Linux client for the classic Clan Lord MMORPG. Includes modern rendering and audio, session recording and playback, legacy macros, Go scripting, and optional text-to-speech. [Website & downloads](https://gothoom.m45sci.xyz/) |
| [EvenAudio](https://github.com/Distortions81/EvenAudio) | Linux desktop audio compressor with seven-band, stereo-linked processing, optional voice leveling, a C audio engine, and a Python/Tk interface for PulseAudio or PipeWire. |
| [goPine](https://github.com/Distortions81/goPineTime) | PineTime smartwatch firmware written in Go with TinyGo. Features clocks, alarms, timers, persistent settings, Bluetooth notifications and music controls, and firmware updates with on-watch confirmation and rollback. An active developer project, with battery runtime still being evaluated. |
| [M45-goPool](https://github.com/M45Core/M45-goPool) | A solo Bitcoin mining pool written from scratch in Go, integrating directly with Bitcoin Core over RPC/ZMQ. Includes Stratum/TLS, worker telemetry, a status dashboard and APIs, operational safeguards, and reproducible benchmarks. [Pool](https://m45core.com/) |
| [StratumStats](https://github.com/M45Core/StratumStats) | Mining-pool observability based on regional Stratum observations: block-template delivery, median and P95 delay, availability, connection timing, TLS, and coinbase-derived fee evidence. Raw observations remain independently recomputable. [Dashboard](https://stratumstats.m45core.com/) |
| [M45-Gamma-Firmware](https://github.com/M45Core/M45-Gamma-Firmware) | ESP32-S3 firmware for Bitaxe Gamma 602 miners. Combines weighted multi-pool share splitting, ordered backup pools, a live dashboard, web updates, hardware diagnostics, and safety controls. |
| [ChatWire](https://github.com/M45-Science/ChatWire) | Factorio server management and Discord integration, covering chat bridging, moderation, process lifecycle control, updates, player databases, and shared multi-instance deployments. |
| [M45-Core-Firmware](https://github.com/M45Core/M45-Core-Firmware) | Classic ESP32 mining firmware with Stratum, hardware SHA candidate loops, a display UI, local setup, statistics, and settings pages. |
| [StratumScout](https://github.com/M45Core/StratumScout) | Regional measurement probes for StratumStats, performing bounded Stratum observations and uploading authenticated batches without submitting shares. |
| [GoMUD2](https://github.com/Distortions81/GoMUD2) | Go MUD server with telnet, optional TLS, ANSI rendering, in-game world editing, and player, builder, and administrator roles. |
| [FactMapGen](https://github.com/M45-Science/FactMapGen) | A Go web editor for Factorio map-generation settings. Includes seeded previews for Nauvis and Space Age planets, exact Factorio rendering, guest workspaces, and authenticated, audited presets. [Try it](https://mapgen.m45sci.xyz/) |

## Project snapshots

Snapshots from across my public and private projects. Private projects are shown without repository links.

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
      <a href="https://github.com/M45Core/M45-goPool">
        <img src="assets/project-thumbnails/m45-gopool.png" alt="M45-goPool dashboard thumbnail" width="150"><br>
        <sub>M45-goPool</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/M45Core/M45-Core-Firmware">
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
        <img src="assets/project-thumbnails/eui.png" alt="EUI demo thumbnail" width="150"><br>
        <sub>EUI</sub>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/Distortions81/PixelPirates">
        <img src="assets/project-thumbnails/pixelpirates.png" alt="PixelPirates gameplay thumbnail" width="150"><br>
        <sub>PixelPirates</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/M45-Science/FactMapGen">
        <img src="assets/project-thumbnails/factmapgen.png" alt="FactMapGen editor and map preview thumbnail" width="150"><br>
        <sub>FactMapGen</sub>
      </a>
    </td>
  </tr>
  <tr>
    <td align="center" width="20%">
      <img src="assets/project-thumbnails/encore-4a.png" alt="Encore-4A sidecar VDP shadow output thumbnail" width="150"><br>
      <sub>Encore-4A</sub>
    </td>
    <td align="center" width="20%">
      <img src="assets/project-thumbnails/project-retrace.png" alt="Project-Retrace MC68000 monitor thumbnail" width="150"><br>
      <sub>Project-Retrace</sub>
    </td>
    <td align="center" width="20%">
      <img src="assets/project-thumbnails/vectorfpga.png" alt="VectorFPGA 3D Doom vector-rendering thumbnail" width="150"><br>
      <sub>VectorFPGA</sub>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/M45Core/M45-Gamma-Firmware">
        <img src="assets/project-thumbnails/m45-gamma-firmware.png" alt="M45-Gamma-Firmware dashboard thumbnail" width="150"><br>
        <sub>M45-Gamma-Firmware</sub>
      </a>
    </td>
    <td align="center" width="20%">
      <a href="https://github.com/M45Core/StratumStats">
        <img src="assets/project-thumbnails/stratumstats.png" alt="StratumStats Bitcoin mining-pool performance dashboard" width="150"><br>
        <sub>StratumStats</sub>
      </a>
    </td>
  </tr>
</table>

## Communities & operations

**[M45-Science](https://github.com/M45-Science)** is where my Factorio community
and server-operations work lives. The public tooling spans Discord integration,
moderation, server orchestration, community lists, downloads, and map management.
ChatWire and FactMapGen are two parts of that wider stack.
[Community website](https://m45sci.xyz/)

**[M45Core](https://github.com/M45Core)** brings together my Bitcoin mining
software, firmware, and observability work. Its projects cover pool servers,
ESP32 and ASIC miner firmware, and distributed regional measurement.

## More public work

- **Games:** [PixelPirates](https://github.com/Distortions81/PixelPirates) and [GoblinSiege](https://github.com/Distortions81/GoblinSiege).
- **Audio & libraries:** [go-meltysynth](https://github.com/Distortions81/go-meltysynth), [ImpSynth](https://github.com/Distortions81/ImpSynth), [GoBeep86](https://github.com/Distortions81/GoBeep86), [go-g726](https://github.com/Distortions81/go-g726), and [goXA](https://github.com/Distortions81/goXA).
- **Linux & practical tools:** [DaVinci-Resolve-Container](https://github.com/Distortions81/DaVinci-Resolve-Container), [Canon-Webcam-Linux](https://github.com/Distortions81/Canon-Webcam-Linux), and [PCB-Frame](https://github.com/Distortions81/PCB-Frame).
- **Math & visualization:** [OpenCLFrac](https://github.com/Distortions81/OpenCLFrac), [golang-frac](https://github.com/Distortions81/golang-frac), and [StrangeAttractors](https://github.com/Distortions81/StrangeAttractors).

[Browse my public repositories →](https://github.com/Distortions81?tab=repositories)

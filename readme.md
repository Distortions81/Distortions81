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


### Links
- [Project Gallery](https://m45sci.xyz/u/dist/)
- [M45-Science GitHub](https://github.com/orgs/M45-Science/repositories)
- [m45core.com](https://m45core.com)

---

## Featured Projects
A selection of repositories that reflect the range of systems, tools, and experiments I work on, ordered roughly by complexity, scope, and technical depth.

### [GD-DOOM](https://github.com/Distortions81/GD-DOOM)
**Language:** Go | **Complexity:** Very High

Go-based Doom engine covering WAD loading, gameplay systems, rendering, audio, UI flow, and demo tooling. It preserves classic Doom behavior, while also offering an optional modernized mode with 32-bit color, higher resolutions, improved audio, and other quality-of-life upgrades.

*Lines of Code:* ~81k

### [goThoom](https://github.com/Distortions81/goThoom)
**Language:** Go | **Complexity:** High

Modern open-source client for the classic Clan Lord MMORPG. Cross-platform desktop application built on Ebiten with OpenGL, DirectX, and Metal rendering, plus plugin support.

*Lines of Code:* ~55k

**Highlights:**
- Cross-platform desktop client built on Ebiten with OpenGL, DirectX, and Metal backends
- Plugin system powered by Yaegi for runtime extensibility and experimentation
- Quality-of-life upgrades including text-to-speech and automatic asset fetching
- Performance-focused rendering improvements, including de-dithering for legacy graphics

### [M45-goPool](https://github.com/Distortions81/M45-goPool)
**Language:** Go | **Complexity:** High

Standalone Bitcoin mining pool designed to pair with Bitcoin Core over JSON-RPC and ZMQ, serve Stratum v1 miners over plain TCP or TLS, expose an HTTPS-first status UI and JSON API, manage TLS certificates automatically, and provide thorough configuration, operations, and testing documentation.

*Lines of Code:* ~50k (including tests)

**Highlights:**
- Deep Bitcoin Core integration via JSON-RPC longpoll + ZMQ block feed for Stratum v1 mining
- Production-minded pool controls: rate limiting, invalid-share bans, reconnect churn mitigation, and TLS support
- Configurable coinbase split handling for fees, donations, and miner payouts
- Strong ops/testing ergonomics with install scripts, profiling helpers, and detailed `operations.md`, `performance.md`, and `TESTING.md`

### [ChatWire](https://github.com/M45-Science/ChatWire)
**Language:** Go | **Complexity:** High

A long-running bridge between Discord and Factorio servers that supports server management and moderation workflows.
Part of the [M45-Science](https://github.com/M45-Science) GitHub organization ([website](https://m45sci.xyz/)).
Active since 2017.

*Lines of Code:* ~16.1k

**Highlights:**
- Long-running Discord-to-Factorio bridge built with [DiscordGo](https://github.com/bwmarrin/discordgo)
- Server orchestration and process control for managing multiple game instances
- Custom game/mod update workflows using the Factorio [Download API](https://wiki.factorio.com/Download_API) and [Mod Portal API](https://wiki.factorio.com/Mod_portal_API)
- Real-time operations tooling with WebSockets, HTTP APIs, and live logging/diagnostics

### [ONI-SeedView](https://github.com/Distortions81/ONI-SeedView)
**Language:** Go | **Complexity:** Medium

WebAssembly map seed viewer for [Oxygen Not Included](https://www.klei.com/games/oxygen-not-included) built with [Ebiten](https://ebitengine.org/). It retrieves [seed data](https://mapsnotincluded.org/) and renders an interactive map with detailed biome and object information.

[Try it here](https://m45sci.xyz/u/dist/oni-view/view.html?coord=SNDST-A-1-0-0-0)
*Lines of Code:* ~5.6k

**Highlights:**
- Parses and visualizes ONI seed data in-browser using Go + WebAssembly
- Interactive map exploration with detailed overlays and adjustable UI scaling
- Export support for high-resolution printable maps
- Mobile-friendly touch controls and alternate viewer integration on [MapsNotIncluded.org](https://mapsnotincluded.org/map-explorer/SNDST-A-1-0-0-0)

### Factorio [SoftMod](https://github.com/M45-Science/SoftMod) (for [M45-Science](https://github.com/M45-Science))
**Language:** Lua | **Complexity:** Medium-High

Scenario scripting for M45-Science Factorio servers, focused on softmod-style server administration and gameplay support.

*Lines of Code:* ~9.5k

**Highlights:**
- Scenario-based server scripting with no client-side mod download required
- Dynamic GUI systems and permission-based commands for moderation/admin workflows
- Player-driven moderation features (including vote-banish) and action logging
- Localization support across multiple languages with live server usage in production

### [PixelPirates](https://github.com/Distortions81/PixelPirates)
**Language:** Go | **Complexity:** Medium-Low

Retro sailing and exploration prototype centered on rendering experiments and gameplay feel.

[Play online](https://m45sci.xyz/u/dist/pixelpirate)
*Lines of Code:* ~5.3k
[Blog post about this project](https://carlotto81.wixsite.com/m45-science/post/solo-game-developer-adventures)

**Highlights:**
- Custom real-time music synthesizer
- Perlin noise-driven procedural sky generation
- Runs well in-browser via WebAssembly
- Can import sprite sheets from [Aseprite](https://www.aseprite.org/)

### [ImpSynth](https://github.com/Distortions81/ImpSynth)
**Language:** Go | **Complexity:** Medium

Compact OPL3-style FM synthesis library in Go focused on the practical DMX/Doom-era register subset: 2-operator voices, envelopes, feedback, waveforms, stereo panning, and direct OPL-style register writes.

*Lines of Code:* ~1k

**Highlights:**
- Focused FM synth implementation tuned around the classic Doom/DMX-style OPL workflow
- Simple register-driven API with stereo `int16` PCM generation
- Includes an example renderer that converts melody CSV + patch JSON inputs into `.wav` output
- Zero-allocation PCM benchmark noted in the repo docs for real-time-friendly synthesis work

### [numfmt](https://github.com/Distortions81/numfmt)
**Language:** Go | **Complexity:** Medium-Low

Compact numeric encoding library for large positive values that trades exactness for predictable error bounds, reducing the size of telemetry, snapshots, and other high-volume numeric payloads.

*Lines of Code:* ~1.5k

**Highlights:**
- Encodes values into compact `8`/`16`/`32` bit integer codes using tunable exponent and mantissa sizing
- Supports constrained ranges and automatic exponent sizing for domain-specific quantization
- Includes a binary payload format for packing whole numeric slices with self-describing codec metadata
- Ships with a small JavaScript codec plus generated quantization-guide docs for cross-language use and evaluation

### [goXA](https://github.com/Distortions81/goXA)
**Language:** Go | **Complexity:** Medium-Low

Custom archiving utility built around a compact archive format.

*Lines of Code:* ~4.9k

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
*Lines of Code:* ~1.7k

**Highlights:**
- Data synchronization
- CLI tool design
- JSON processing
- Lightweight web server

### [FactorioServerBrowser](https://github.com/M45-Science/FactorioServerBrowser)
**Language:** Go | **Complexity:** Medium-Low

Minimal Factorio server browser with a web interface. Polls servers on a schedule, caches results, and serves a simple index page.

[Live Demo](https://factorio.go-game.net/)
*Lines of Code:* ~1.1k

**Highlights:**
- RESTful HTTP handling
- Server polling and caching
- Front-end/back-end integration
- Uses [matchmaking](https://wiki.factorio.com/Matchmaking_API) API

### [GoRecoverBlurText](https://github.com/Distortions81/GoRecoverBlurText)
**Language:** Go | **Complexity:** Medium
Experimental tool that attempts to recover blurred or pixelated text through brute-force comparison.
*Lines of Code:* ~360

### [golang-frac](https://github.com/Distortions81/golang-frac)
**Language:** Go | **Complexity:** Medium
Mandelbrot fractal renderer for high-detail image and video frame generation.

*Lines of Code:* ~380

**Highlights:**
- Multi-threaded Mandelbrot rendering
- High-resolution frame/image generation
- CLI-controlled zoom and render parameters

### [goMarketMadness](https://github.com/Distortions81/goMarketMadness)
**Language:** Go | **Complexity:** Medium
A tribute to a childhood type-in economic simulation, reimplemented in Go.

[Play it here](https://m45sci.xyz/u/dist/otto/marketmadness/)
*Lines of Code:* ~1.7k

**Highlights:**
- Simulates TUI of TI-99/4a
- Game loop and economic modeling (Brownian noise)
- Event-driven simulation

_Thank you for visiting._

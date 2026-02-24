<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=header&text=Distortions81&fontSize=48&fontColor=ffffff" alt="Carl Otto Header"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?lines=Systems+programming+meets+game+dev;Always+building+something+new!&center=true&width=440&height=35" alt="Typing SVG" />
</p>

## About Me

I work across software, electronics, and data, with a focus on systems programming, game development, automation, and infrastructure-oriented tooling. My projects often combine implementation with measurement, using benchmarks, visualizations, and prototypes to make trade-offs explicit.  

I approach projects iteratively: build, measure, refine, and document. Some repositories are production-ready tools, while others are focused experiments used to validate a design or technical approach.  

I value efficiency and leverage: automation scripts, clear formats, and practical tooling that reduce friction between an idea and a working system.  

In practice, that means building systems, inspecting how they behave, and improving them until they are reliable, understandable, and useful.


### Links
- [Project Gallery](https://m45sci.xyz/u/dist/)
- [M45-Science GitHub](https://github.com/orgs/M45-Science/repositories)
- [m45core.com](https://m45core.com)

---

## Featured Projects
A selection of repositories that showcase what I like to build.

### [goThoom](https://github.com/Distortions81/goThoom)
**Language:** Go | **Complexity:** High

Modern open-source client for the classic Clan Lord MMORPG. Cross-platform binary using the Ebiten game engine with OpenGL, DirectX, or Metal rendering and plugin support.

*Lines of Code:* ~55k

**Highlights:**
- Cross-platform desktop client built on Ebiten with OpenGL, DirectX, and Metal backends
- Plugin system powered by Yaegi for runtime extensibility and experimentation
- Quality-of-life upgrades including text-to-speech and automatic asset fetching
- Performance-focused rendering improvements, including de-dithering for legacy graphics

### [M45-goPool](https://github.com/Distortions81/M45-goPool)
**Language:** Go | **Complexity:** High

Standalone Bitcoin mining pool that pairs with Bitcoin Core (JSON-RPC + ZMQ) to serve Stratum v1 miners (plain or TLS), exposes an HTTPS-first status UI/JSON API, auto-manages TLS certs, and packages rich config, operations, and testing docs.

*Lines of Code:* ~50k (including tests)

**Highlights:**
- Deep Bitcoin Core integration via JSON-RPC longpoll + ZMQ block feed for Stratum v1 mining
- Production-minded pool controls: rate limiting, invalid-share bans, reconnect churn mitigation, and TLS support
- Configurable coinbase split handling for fees, donations, and miner payouts
- Strong ops/testing ergonomics with install scripts, profiling helpers, and detailed `operations.md`, `performance.md`, and `TESTING.md`

### [ChatWire](https://github.com/M45-Science/ChatWire)
**Language:** Go | **Complexity:** High

A robust bridge between Discord and Factorio servers that manages game servers and empowers moderators.
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

WebAssembly map seed viewer for [Oxygen Not Included](https://www.klei.com/games/oxygen-not-included) built with [Ebiten](https://ebitengine.org/). It fetches [seed data](https://mapsnotincluded.org/) and renders an interactive map with detailed biome/object information.

[Try it here](https://m45sci.xyz/u/dist/oni-view/view.html?coord=SNDST-A-1-0-0-0)
*Lines of Code:* ~5.6k

**Highlights:**
- Parses and visualizes ONI seed data in-browser using Go + WebAssembly
- Interactive map exploration with detailed overlays and adjustable UI scaling
- Export support for high-resolution printable maps
- Mobile-friendly touch controls and alternate viewer integration on [MapsNotIncluded.org](https://mapsnotincluded.org/map-explorer/SNDST-A-1-0-0-0)

### [goXA](https://github.com/Distortions81/goXA)
**Language:** Go | **Complexity:** Medium-Low

Custom archiving utility with a compact format.

*Lines of Code:* ~4.9k

**Highlights:**
- Custom archive structure
- Checksums, many compression types
- Preserve file permissions, mod times
- Offers forward error correction
- Threaded compression options

### Factorio [SoftMod](https://github.com/M45-Science/SoftMod) (for [M45-Science](https://github.com/M45-Science))
**Language:** Lua | **Complexity:** Medium-High

Scenario scripts for M45-Science Factorio servers (softmod/scenario scripting).

*Lines of Code:* ~9.5k

**Highlights:**
- Scenario-based server scripting with no client-side mod download required
- Dynamic GUI systems and permission-based commands for moderation/admin workflows
- Player-driven moderation features (including vote-banish) and action logging
- Localization support across multiple languages with live server usage in production

### [PixelPirates](https://github.com/Distortions81/PixelPirates)
**Language:** Go | **Complexity:** Medium-Low

Retro sailing and exploration prototype focused on rendering and game-feel experimentation.

[Play online](https://m45sci.xyz/u/dist/pixelpirate)
*Lines of Code:* ~5.3k
[Blog post about this project](https://carlotto81.wixsite.com/m45-science/post/solo-game-developer-adventures)

**Highlights:**
- Custom real-time music synthesizer
- Perlin noise-driven procedural sky generation
- Runs well in-browser via WebAssembly
- Can import sprite sheets from [Aseprite](https://www.aseprite.org/)

### [goMMO](https://github.com/Distortions81/goMMO)
**Language:** Go | **Complexity:** Medium-Low

Client-side MMO prototype demonstrating basic networking. Implements a small world simulation and WebSocket communication for testing.

*Lines of Code:* ~5.1k

**Highlights:**
- WebSocket networking
- Custom low-bandwidth binary networking protocol
- Linear interpolation for smooth movement/frame pacing at low update rates (8 Hz base)
- Hashmap-backed chunk system for efficient world state management
- Serialized game-data caching to reduce CPU load in busy areas

### [FactorioServerBrowser](https://github.com/M45-Science/FactorioServerBrowser)
**Language:** Go | **Complexity:** Medium-Low

Minimal server browser for Factorio with a web interface. Polls servers on a schedule, caches results, and serves a simple index page.

[Live Demo](https://factorio.go-game.net/)
*Lines of Code:* ~1.1k

**Highlights:**
- RESTful HTTP handling
- Server polling and caching
- Front-end/back-end integration
- Uses [matchmaking](https://wiki.factorio.com/Matchmaking_API) API

### [FactBanSync](https://github.com/M45-Science/FactBanSync)
**Language:** Go | **Complexity:** Medium

Synchronizes ban lists across multiple Factorio servers. Contains a CLI merge tool and lightweight web API for centralized management.

[Web Interface](https://m45sci.xyz:8443/)
*Lines of Code:* ~1.7k

**Highlights:**
- Data synchronization
- CLI tool design
- JSON processing
- Lightweight web server

### [GoRecoverBlurText](https://github.com/Distortions81/GoRecoverBlurText)
**Language:** Go | **Complexity:** Medium
Experimental tool that attempts to recover blurred or pixelated text using brute-force comparison.
*Lines of Code:* ~360

### [golang-frac](https://github.com/Distortions81/golang-frac)
**Language:** Go | **Complexity:** Medium
Mandelbrot fractal renderer for high-detail image/video frame generation.

*Lines of Code:* ~380

**Highlights:**
- Multi-threaded Mandelbrot rendering
- High-resolution frame/image generation
- CLI-controlled zoom and render parameters

### [goMarketMadness](https://github.com/Distortions81/goMarketMadness)
**Language:** Go | **Complexity:** Medium
A tribute to a childhood type-in economic simulation.

[Play it here](https://m45sci.xyz/u/dist/otto/marketmadness/)
*Lines of Code:* ~1.7k

**Highlights:**
- Simulates TUI of TI-99/4a
- Game loop and economic modeling (Brownian noise)
- Event-driven simulation

## GitHub Stats
![Stats](https://github-readme-stats.vercel.app/api?username=Distortions81&show_icons=true&theme=dark)

_Thank you for visiting._

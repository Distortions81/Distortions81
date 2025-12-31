<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=header&text=Distortions81&fontSize=48&fontColor=ffffff" alt="Carl Otto Header"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?lines=Systems+programming+meets+game+dev;Always+building+something+new!&center=true&width=440&height=35" alt="Typing SVG" />
</p>

## About Me

I’m a builder at heart. I move fluidly between code, electronics, and data—whether it’s writing Go servers and game engines, hacking Factorio mods, tuning Linux systems, or modeling solar batteries. I like to peel back abstractions, test assumptions, and make trade-offs visible with graphs, benchmarks, and prototypes.  

I treat every project as an experiment: build, measure, refine, repeat. My repos reflect that tinkerer-scientist loop—sometimes it’s a polished tool, other times it’s a weird prototype that scratches an itch. Either way, it’s hands-on, data-driven, and open to exploration.  

I value efficiency and leverage: scripts that automate, formats that clarify, visualizations that reveal. If there’s friction between an idea and a working system, I want to sand it down.  

In short: I don’t just use systems—I take them apart, rebuild them, and see how far they can be pushed.


### 🌐 Links
- [🔥Project Gallery](https://m45sci.xyz/u/dist/)
- [📝 Blog Posts](https://carlotto81.wixsite.com/m45-science)
- [✨ M45-Science Hub](https://m45sci.xyz/)
- [🏢 M45-Science GitHub](https://github.com/orgs/M45-Science/repositories)
- [🕸️ m45core.com](https://m45core.com)
- [🎮 go-game.net](http://go-game.net)
---

## 🌟 Featured Projects
A selection of repositories that showcase what I like to build.

### ⚔️ [goThoom](https://github.com/Distortions81/goThoom)
**Language:** Go | **Complexity:** High

Modern open-source client for the classic Clan Lord MMORPG. Cross-platform binary using the Ebiten game engine with OpenGL, DirectX, or Metal rendering and plugin support.

*Lines of Code:* ~45k

**Highlights:**
- Cross-platform builds with fast Ebiten rendering (OpenGL/DirectX/Metal)
- Text-to-speech and asset auto-fetch
- Plugin system powered by Yaegi
- Higher framerates with de-dithering of legacy graphics

### 🏦 [M45-Core-goPool](https://github.com/Distortions81/M45-Core-goPool)
**Language:** Go | **Complexity:** High

Standalone Bitcoin mining pool that pairs with Bitcoin Core (JSON-RPC + ZMQ) to serve Stratum v1 miners (plain or TLS), exposes an HTTPS-first status UI/JSON API, auto-manages TLS certs, and packages rich config, operations, and testing docs.

**Highlights:**
- Bitcoin Core integration (RPC longpoll and ZMQ block feed) with configurable coinbase splits for fee, donation, and miner payouts.
- Defensive controls for rate limiting, invalid-submission bans, reconnect churn mitigation, and live reload signals for templates/config.
- Scripts for installing Bitcoin Core, running the full Go test suite, profiling CPU usage, plus detailed `operations.md`/`performance.md`/`TESTING.md`.

### 🚀 [ChatWire](https://github.com/M45-Science/ChatWire)
**Language:** Go | **Complexity:** High

A robust bridge between Discord and Factorio servers, manages servers and empowers moderators.
A part of [M45-Science](https://github.com/M45-Science) github organization ([Website](https://m45sci.xyz/)).
Active since 2017.

*Lines of Code:* ~14.2k

**Highlights:**
- Discord bot development: [DiscordGo](https://github.com/bwmarrin/discordgo)
- Custom game-server and game-mod updaters. [Download API](https://wiki.factorio.com/Download_API), [Mod API](https://wiki.factorio.com/Mod_portal_API)
- Go concurrency and goroutines
- Process control and system integration
- WebSockets and HTTP APIs
- Live logging and diagnostics

### 👀 [ONI-SeedView](https://github.com/Distortions81/ONI-SeedView)
**Language:** Go | **Complexity:** Medium

Web (web assembly) map seed viewer for the game '[Oxygen Not Included](https://www.klei.com/games/oxygen-not-included)' using [Ebiten](https://ebitengine.org/). Fetches [seed data](https://mapsnotincluded.org/) and renders an interactive map with detailed info.

[Try it here](https://m45sci.xyz/u/dist/oni-view/view.html?coord=SNDST-A-1-0-0-0)
*Lines of Code:* ~4.6k

**Highlights:**
- Game data parsing
- Rendering with Ebiten
- Interactive seed exploration
- UI scale can be adjusted
- Can export high-res printable maps
- Touch controls for mobile
- Available as an alternate viewer on [MapsNotIncluded.org](https://mapsnotincluded.org/map-explorer/SNDST-A-1-0-0-0)

### 📦 [goXA](https://github.com/Distortions81/goXA)
**Language:** Go | **Complexity:** Medium-Low

Custom archiving utility with a compact format.

 *Lines of Code:* ~5.0k

**Highlights:**
- Custom archive structure
- Checksums, many compression types
- Preserve file permissions, mod times
- Offers forward error correction
- Threaded compression options

### 🛠️ Factorio [SoftMod](https://github.com/M45-Science/SoftMod) (for [M45-Science](https://github.com/M45-Science))
**Language:** Lua | **Complexity:** Medium-High

*Lines of Code:* ~7.5k

**Highlights:**
- Localized to several languages
- Player menu with vote-banish system for player-based moderation.
- No game mod download needed
- Can be updated mid-game via careful use of scenario scripting
- Dynamic GUI generation
- Permission-based commands
- Player permissions management
- Logging of player actions

### 🏴‍☠️ [PixelPirates](https://github.com/Distortions81/PixelPirates)
**Language:** Go | **Complexity:** Medium-Low

Retro sailing and exploration prototype.

[Play online](https://m45sci.xyz/u/dist/pixelpirate)
*Lines of Code:* ~5.7k
[Blog post about this project](https://carlotto81.wixsite.com/m45-science/post/solo-game-developer-adventures)

**Highlights:**
- Custom real time music synthesizer.
- Use of Perlin Noise for procedural generation of sky.
- Runs well in-browser using web assembly.
- Can imort sprite sheets from [Aseprite](https://www.aseprite.org/)

### 🕹️ [goMMO](https://github.com/Distortions81/goMMO)
**Language:** Go | **Complexity:** Medium-Low

Client-side MMO prototype demonstrating basic networking. Implements a small world simulation and WebSocket communication for testing.

*Lines of Code:* ~3.9k

**Highlights:**
- WebSocket networking
- Custom low-bandwith binary networking protocol
- Use of linear interpolation for smooth movement and frame-rate, even with base rate of 8 updates per second.
- Uses hashmap map-chunk system for efficiency 
- Caching of serialized game data to significantly reduce CPU needed in busy areas

### 🌐 [FactorioServerBrowser](https://github.com/M45-Science/FactorioServerBrowser)
**Language:** Go | **Complexity:** Medium-Low

Minimal server browser for Factorio with a web interface. Polls servers on a schedule, caches results, and serves a simple index page.

[Live Demo](https://factorio.go-game.net/)
*Lines of Code:* ~1.3k

**Highlights:**
- RESTful HTTP handling
- Server polling and caching
- Front-end/back-end integration
- Uses [matchmaking](https://wiki.factorio.com/Matchmaking_API) API

### 🚫 [FactBanSync](https://github.com/M45-Science/FactBanSync)
**Language:** Go | **Complexity:** Medium

Synchronizes ban lists across multiple Factorio servers. Contains a CLI merge tool and lightweight web API for centralized management.

[Web Interface](https://m45sci.xyz:8443/)
*Lines of Code:* ~1.7k

**Highlights:**
- Data synchronization
- CLI tool design
- JSON processing
- Lightweight web server

### 📚 [GoRecoverBlurText](https://github.com/Distortions81/GoRecoverBlurText)
**Language:** Go | **Complexity:** Medium
Attempts to recover blurred or pixelated text using brute-force comparison that is surprisingly effective.
*Lines of Code:* ~330

### 🌀 [golang-frac](https://github.com/Distortions81/golang-frac)
**Language:** Go | **Complexity:** Medium
Fractal visualizer and generator with WebAssembly support.

*Lines of Code:* ~300

**Highlights:**
- Complex number math
- Ebiten graphics engine
- WASM build pipeline

### 💹 [goMarketMadness](https://github.com/Distortions81/goMarketMadness)
**Language:** Go | **Complexity:** Medium
A tribute to a childhood type-in economic sim.

[Play it here](https://m45sci.xyz/u/dist/otto/marketmadness/)
 *Lines of Code:* ~1.9k

**Highlights:**
- Simulates TUI of TI-99/4a
- Game loop and economic modeling (brownian noise)
- Event-driven simulation

## 📈 GitHub Stats
![Stats](https://github-readme-stats.vercel.app/api?username=Distortions81&show_icons=true&theme=dark)

_Thanks for visiting!_

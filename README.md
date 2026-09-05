<!--
  ____                       _    _    ___
 |  _ \ __ _ ___  ___ __ _  | |  / \  |_ _|
 | |_) / _` / __|/ __/ _` | | | / _ \  | |
 |  __/ (_| \__ \ (_| (_| | | |/ ___ \ | |
 |_|   \__,_|___/\___\__,_| |_/_/   \_\___|

  Ingenious Digital · Fort Lauderdale · (954) 834-3426
  pascal@ingeniousdigital.com
-->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/header-dark-v4.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/header-light-v4.svg">
    <img alt="PascalAI / Ingenious Digital — websites, shopify, wordpress, CRM, automations, AI agents, MCP servers, LLM research, CUDA kernels, firmware, games, 3D real-time, VPN and infra, data pipelines, lead gen" src="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/header-dark-v4.svg" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://ingeniousdigital.com">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=21&pause=1300&color=47D7FF&center=true&vCenter=true&width=820&lines=Client+sites+and+storefronts+that+have+to+convert.;Shopify+themes%2C+WordPress+builds%2C+SEO%2C+lead+funnels.;Then+CUDA+kernels+and+ESP32+firmware+after+hours.;Fort+Lauderdale.+Shipping+worldwide." alt="Client sites and storefronts that have to convert. Shopify themes, WordPress builds, SEO, lead funnels. Then CUDA kernels and ESP32 firmware after hours. Fort Lauderdale, shipping worldwide.">
  </a>
</p>

<p align="center">
  <a href="https://ingeniousdigital.com"><b>Ingenious Digital</b></a> ·
  <a href="https://ingeniousdigital.com/services">Services</a> ·
  <a href="https://igddev.com">IGD Dev Lab</a> ·
  <a href="https://github.com/PascalAI2024/portfolio">Portfolio</a> ·
  <a href="mailto:pascal@ingeniousdigital.com"><b>pascal@ingeniousdigital.com</b></a>
</p>

---

I run **[Ingenious Digital](https://ingeniousdigital.com)**, a product studio in
Fort Lauderdale. Most weeks that means client websites, Shopify storefronts,
WordPress builds, SEO and lead funnels, CRM and automation work — the systems a
business actually runs on.

The rest of the time it's GPU kernels, Zig shells, ESP32 firmware and agent
infrastructure, which is where most of this GitHub comes from.

---

## JarvisMCP — one gateway, two tools

**Flagship infrastructure for the studio. Closed-source.**

Most agent setups bolt on an MCP server per integration and drown the model in
tool definitions before it does any work. This inverts it. The agent gets **two**
tools — search and execute — writes JavaScript against them, and the catalogue
stays server-side.

<table>
<tr>
<td align="center"><b>2</b><br/><sub>tools exposed</sub></td>
<td align="center"><b>Search</b><br/><sub>discover capabilities</sub></td>
<td align="center"><b>Execute</b><br/><sub>compose work</sub></td>
<td align="center"><b>Leases</b><br/><sub>coordinate ownership</sub></td>
<td align="center"><b>Checkpoints</b><br/><sub>resume work</sub></td>
</tr>
</table>

Capability lookup happens before execution. Agent-authored code runs in a
sandboxed isolate holding no credentials, and the services that do hold them sit
outside that boundary. A durable coordination board keeps ownership,
leases, checkpoints and evidence attached to the work across agents, sessions
and computers. The public firmware project, JarvisNano, is separate from this
private gateway.

```mermaid
flowchart TB
    A["Coding agent"] -->|"1 search"| C["Capability catalogue<br/>Discoverable services"]
    C -.->|"signature"| A
    A -->|"2 execute"| S["Sandboxed isolate<br/>no credentials"]
    S -->|"bounded call"| G["Gateway"]
    G <--> V["Credential-holding services"]
    S -->|"result"| A
    H["Person"] -->|"approves writes"| G
```

[Public architecture story](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/jarvismcp.md) · Source and operational details remain private.

---

## Open source

<table>
<tr>
<td width="50%" valign="top">

### 🧪 [fplbench](https://github.com/PascalAI2024/fplbench)

A leakage-aware Fantasy Premier League dataset and forecasting system. The
forecast is committed before the deadline, the model plays its own public team,
and automation grades the frozen forecast after verified gameweek results.

`Python` · MIT code; separate data terms · [dataset](https://huggingface.co/datasets/x0me/fplbench) · [live board](https://huggingface.co/spaces/x0me/fplbench-board)

</td>
<td width="50%" valign="top">

### ⚡ [Maple CUDA](https://github.com/PascalAI2024/maple-preview-windows-cuda)

Seven local CUDA patches that made a 20B‑A1B ternary model practical on a 16 GB
GPU under Windows. Generation 52 → 377 tok/s, prompt processing 1,457 → 10,674
tok/s, against a 103-case CPU-reference matrix. These published experiments
are hardware- and revision-specific; the original generation run and later
prompt-processing reproduction are documented separately.

`CUDA` · [benchmarks](https://huggingface.co/datasets/x0me/maple-preview-cuda-benchmarks) · [case study](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/maple-cuda.md)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🐚 [ZiggyZag](https://github.com/PascalAI2024/ZiggyZag)

An all-Zig shell workspace: a readable shell core, native Windows and macOS
terminal hosts, a cross-platform launcher, and a local AI sidecar. The agent
proposes mutations; the host owns the approval.

`Zig` · [releases](https://github.com/PascalAI2024/ZiggyZag/releases)

</td>
<td width="50%" valign="top">

### 🤖 [JarvisNano](https://github.com/PascalAI2024/JarvisNano)

ESP32-S3 firmware for the Waveshare Touch AMOLED 1.75C desk companion: round
display, touch, live voice, device diagnostics, and a guarded tool bridge.
Public firmware, with hardware release gates still in progress.

`C` · `ESP-IDF` · [architecture](https://github.com/PascalAI2024/JarvisNano/blob/main/docs/ARCHITECTURE.md)

</td>
</tr>
</table>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/bench-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/bench-light.svg">
    <img alt="Maple CUDA measured throughput: generation 52 to 377 tokens per second (7.2x), prompt processing 1,457 to 10,674 tokens per second (7.3x), 103 of 103 CPU-reference cases passed" src="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/bench-dark.svg" width="100%">
  </picture>
</p>

| Project | Lane | Status |
| :-- | :-- | :-- |
| [fplbench](https://github.com/PascalAI2024/fplbench) | Applied ML / data | Live 2026/27 benchmark |
| [Maple CUDA](https://github.com/PascalAI2024/maple-preview-windows-cuda) | GPU performance | v1.0 release + post-release MMQ research |
| [Qwen Quant Bench](https://github.com/PascalAI2024/qwen38-27b-quant-bench) | LLM research | Completed research record |
| [ZiggyZag](https://github.com/PascalAI2024/ZiggyZag) | Native dev tools | Active alpha |
| [JarvisNano](https://github.com/PascalAI2024/JarvisNano) | Embedded AI | Hardware release candidate |
| [PicoArmy](https://github.com/PascalAI2024/picoarmy) | Agent fleets | Public prototype, no deployment |
| [Verrow](https://github.com/PascalAI2024/verrow) | Data operations | Public prototype |
| [KinTunnel](https://github.com/PascalAI2024/kintunnel) | Self-hosted networking | Runnable MVP, dry-run default |

[Case studies](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/README.md) ·
[capability map](https://github.com/PascalAI2024/portfolio/blob/main/capabilities/README.md) ·
[system shapes](https://github.com/PascalAI2024/portfolio/blob/main/architecture/README.md) ·
[evidence ledger](https://github.com/PascalAI2024/portfolio/blob/main/proof/README.md)

---

## Client work

Live sites, built and maintained by the shop.

| Site | What we built | Stack |
| :-- | :-- | :-- |
| **[Healthy Glow Aesthetics](https://healthyglowaesthetics.com)** | Med spa site and local SEO — treatment discovery and booking | WordPress · SEO |
| **[Healthy Glow Shop](https://shop.healthyglowaesthetics.com)** | Product storefront, custom theme and merchandising | Shopify |
| **[The Fort Lauderdale MedSpa](https://thefortlauderdalemedspa.com)** | Practice site for injectables and skincare, built around booking intent | WordPress · SEO |
| **[Ingenious Digital](https://ingeniousdigital.com)** | The studio's own site — React, TypeScript, 3D, voice assistant, CRM automation | React · TS |

Also: digital marketing, ad management, lead generation, GA4 and CRM wiring,
and post-launch maintenance. Service breakdown at
[ingeniousdigital.com/services](https://ingeniousdigital.com/services).

---

## Products

Selected studio products. Availability and release maturity vary by project.

| | | |
| :-- | :-- | :-- |
| **[ButlerCRM](https://butlercrm.com)** | AI-first CRM for revenue teams | Elixir · Phoenix LiveView |
| **[IGD Games](https://games.igddev.com)** | Playable browser-game lab — circuit puzzles, ant colonies, folklore and tactical prototypes | TypeScript · Phaser · PixiJS · HTML5 |
| **[GlowClient](https://glowclient.com)** | Practice management for medical aesthetics — booking, payments, clients | Full-stack TS |
| **[NexusDialer](https://nexusdialer.com)** | Enterprise contact center with BYOS | Full-stack TS |
| **[TraceKill](https://tracekill.com)** | Data-broker exposure scanning | Full-stack TS |
| **[PolyHuntr](https://polyhuntr.com)** | Copy trading, gated on the math | Full-stack TS |

More out of [IGD Dev Lab](https://igddev.com): **Oxide Studio** (AI dev
environment with multi-model support), **Juba** (investigative dossier builder with a
force-directed knowledge graph), **ZeroChat** (on-device voice agent),
**DataAlchemy**, **TariffSync**, **VocalFrame**, **ZeroInbox**, **CallCue**,
**HVAC Recruit**, **HerCircle**, and a real-time space strategy game with
deterministic combat and orbital mechanics.

**Play the game lab:** [IGD Games](https://games.igddev.com) brings together
**Gizmo Works**, **SubTerra Lite**, **Papardes Zieds**, and other playable
experiments. Builds range from early prototypes to launch candidates; the source
repository is private. [Read the project story](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/igd-games.md).

---

## What we build

| Lane | What that means on a Tuesday |
| :-- | :-- |
| 🌐 **Web, commerce & content** | Marketing sites, Shopify themes, WordPress builds, SEO and lead-gen funnels |
| 📞 **CRM, comms & automation** | CRM platforms, contact-center systems, automation wired into the stack a client already has |
| 📈 **Growth** | Lead capture, SEO, ad management, conversion and reporting wired into GA4 and the CRM |
| 🤖 **AI agents & MCP infrastructure** | Supervised agent fleets, scoped MCP access, audited operations |
| 🔬 **ML & GPU research** | Leakage-safe datasets, CUDA kernel work, sub-2-bit quantization |
| ⚙️ **Native tools & systems** | A Zig shell workspace, a capability-safe agent language, self-hosted WireGuard |
| 🔌 **Embedded & hardware** | ESP32-S3 firmware, AMOLED and voice interfaces, guarded tool bridges |

---

## Stack

<table>
<tr><td><b>Client web<br/>& commerce</b></td><td>
<img src="https://skillicons.dev/icons?i=wordpress,php,js,ts,react,nextjs,tailwind,vite&theme=dark" alt="WordPress, PHP, JavaScript, TypeScript, React, Next.js, Tailwind, Vite" height="48">
<a href="https://shop.healthyglowaesthetics.com"><img src="https://img.shields.io/badge/Shopify-7AB55C?style=for-the-badge&logo=shopify&logoColor=white" alt="Shopify" height="48"></a>
</td></tr>
<tr><td><b>Backend<br/>& data</b></td><td>
<img src="https://skillicons.dev/icons?i=nodejs,bun,nestjs,elixir,python,fastapi,postgres,prisma&theme=dark" alt="Node.js, Bun, NestJS, Elixir, Python, FastAPI, PostgreSQL, Prisma" height="48">
</td></tr>
<tr><td><b>Systems<br/>& embedded</b></td><td>
<img src="https://skillicons.dev/icons?i=rust,go,zig,c,cpp,arduino&theme=dark" alt="Rust, Go, Zig, C, C++, embedded" height="48">
</td></tr>
<tr><td><b>Apps, 3D<br/>& games</b></td><td>
<img src="https://skillicons.dev/icons?i=flutter,dart,threejs,blender,godot&theme=dark" alt="Flutter, Dart, Three.js, Blender, Godot" height="48">
</td></tr>
<tr><td><b>Infra<br/>& tooling</b></td><td>
<img src="https://skillicons.dev/icons?i=docker,nginx,cloudflare,linux,bash,powershell,git,github&theme=dark" alt="Docker, nginx, Cloudflare, Linux, Bash, PowerShell, Git, GitHub" height="48">
</td></tr>
</table>

Plus Traefik, Dokploy, Proxmox, ESP-IDF, CUDA, WireGuard and GA4 — which don't
have icons but do have production hours.

---

## In-house

The studio runs on tooling built for itself. Source-private, so what follows is
the system shape — not the machinery.

### Overwatch — search intelligence as one working surface

Rank tracking, search performance, local visibility and AI-era search signals in
a single self-hosted project view, instead of five specialist dashboards.
Background jobs keep the picture current; the assistant proposes actions and a
human approves them. `Bun` · `TanStack Start` · `PostgreSQL` · `Drizzle`

### ButlerCRM — follow-up that doesn't get dropped

AI-first CRM for revenue teams, running live at
[butlercrm.com](https://butlercrm.com). `Elixir` · `Phoenix LiveView` ·
`PostgreSQL`

### GigaBrain — operating memory you can point an agent at

A knowledge-vault template that ships with structure and **no data** — nothing
project-, client- or person-specific. Point an agent at a copy and it learns the
project's architecture, positioning and history as you fill it in, then keeps it
maintained.

Also public: [PAL](https://github.com/PascalAI2024/pal-lang), an early language
research project with no declared repository license.

### Sandbox fleet

Self-hosted disposable environments so agents can run real work — installs,
builds, migrations — without touching anything that matters.

> Client data, credentials, production topology, security controls, internal
> prompts, service addresses and access paths stay out of public repositories.
> The [boundaries](https://github.com/PascalAI2024/portfolio/blob/main/PUBLIC_BOUNDARIES.md)
> are written down, so the line doesn't get decided case by case.

---

## Also true

- Half my infrastructure is named after a fictional butler.
- A Shopify theme, a Roblox scene and a CUDA kernel can land in the same week of commits.
- The stack runs from `Shopify Liquid` to `ESP-IDF`. Nobody planned that.
- The public portfolio is a selected view of the work, with evidence and project boundaries.

---

## Work together

Websites and storefronts that have to convert. CRMs and automations that have to
hold up. Or the harder end — AI and agent infrastructure, performance work,
research systems, and prototypes that have to become maintainable products.

<p align="center">
  <a href="mailto:pascal@ingeniousdigital.com"><b>pascal@ingeniousdigital.com</b></a> ·
  <a href="https://ingeniousdigital.com/contact"><b>ingeniousdigital.com/contact</b></a> ·
  (954) 834-3426<br>
  <sub>Fort Lauderdale, on Eastern time · shipping worldwide</sub>
</p>

<p align="center">
  <sub>
    <a href="https://ingeniousdigital.com">ingeniousdigital.com</a> ·
    <a href="https://igddev.com">igddev.com</a> ·
    <a href="https://huggingface.co/x0me">huggingface.co/x0me</a> ·
    <a href="https://github.com/PascalAI2024/portfolio">portfolio</a>
  </sub>
</p>

<!--
  You went looking in the source. Respect.
  pascal@ingeniousdigital.com — mention the ASCII art.
-->

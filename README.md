<!--
  ____                       _    _    ___
 |  _ \ __ _ ___  ___ __ _  | |  / \  |_ _|
 | |_) / _` / __|/ __/ _` | | | / _ \  | |
 |  __/ (_| \__ \ (_| (_| | | |/ ___ \ | |
 |_|   \__,_|___/\___\__,_| |_/_/   \_\___|

  You read the source instead of the summary. Good instinct — that's the
  whole method around here. Every claim below this line has a link you can
  open and check. Nothing is measured in adjectives.

  Ingenious Digital · Fort Lauderdale · (954) 834-3426
-->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/header-dark-v2.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/header-light-v2.svg">
    <img alt="PascalAI / Ingenious Digital — websites, shopify, wordpress, CRM, automations, AI agents, MCP servers, LLM research, CUDA kernels, firmware, games, 3D real-time, VPN and infra, data pipelines, lead gen" src="https://raw.githubusercontent.com/PascalAI2024/PascalAI2024/main/assets/header-dark-v2.svg" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://ingeniousdigital.com">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=21&pause=1300&color=47D7FF&center=true&vCenter=true&width=820&lines=Client+websites+by+day.+CUDA+kernels+by+night.;Shopify+themes%2C+Zig+shells%2C+ESP32+firmware+%E2%80%94+same+week.;Fractional+CTO+in+Fort+Lauderdale.+Shipping+worldwide.;Every+number+on+this+page+has+a+link+behind+it." alt="Client websites by day, CUDA kernels by night. Shopify themes, Zig shells, ESP32 firmware in the same week. Fractional CTO in Fort Lauderdale, shipping worldwide. Every number on this page has a link behind it.">
  </a>
</p>

<p align="center">
  <a href="https://ingeniousdigital.com"><b>Ingenious Digital</b></a> ·
  <a href="https://igddev.com">IGD Dev Lab</a> ·
  <a href="https://github.com/PascalAI2024/portfolio">Portfolio</a> ·
  <a href="https://github.com/PascalAI2024/portfolio/blob/main/proof/README.md">Evidence ledger</a> ·
  <a href="https://huggingface.co/x0me">Hugging Face</a> ·
  <a href="https://ingeniousdigital.com/contact"><b>Hire the shop</b></a>
</p>

---

## Hey — I'm Pascal 👋

I run **[Ingenious Digital](https://ingeniousdigital.com)**, a product studio in
Fort Lauderdale, and **[IGD Dev Lab](https://igddev.com)**, where the more
ambitious ideas get built. By day that's fractional CTO work, custom software,
automations, and the websites and CRMs that keep South Florida businesses
running. By night it's GPU kernels, Zig shells, ESP32 firmware, agent fleets and
games — because the interesting problems don't respect job titles.

It looks like a wildly scattered range. It's one habit applied to all of it:

> Turn a fuzzy problem into a thing you can point at · keep the human in charge
> wherever software can do real damage · measure it against a fair baseline ·
> then publish the evidence, the limits, and the current status **together**.

Alpha is called alpha here. That's the whole trick.

---

## What we actually build

| Lane | What that means on a Tuesday | Where to look |
| :-- | :-- | :-- |
| 🌐 **Web, commerce & content** | Marketing sites, Shopify themes, WordPress builds, SEO and lead-gen funnels for businesses with real revenue on the line | [ingeniousdigital.com](https://ingeniousdigital.com) |
| 📞 **CRM, comms & automation** | CRM platforms, contact-center systems, business automation wired into the stack a client already has | [services](https://ingeniousdigital.com/services) |
| 🤖 **AI agents & MCP infrastructure** | Supervised agent fleets, scoped MCP access, audited operations — the agent proposes, a human still approves | [PicoArmy](https://github.com/PascalAI2024/picoarmy) |
| 🔬 **ML & GPU research** | Leakage-safe datasets, CUDA kernel work, sub-2-bit quantization studies — published with the raw numbers *and* the failures | [Hugging Face](https://huggingface.co/x0me) |
| ⚙️ **Native tools & systems** | A Zig shell workspace, a capability-safe agent language, self-hosted WireGuard access | [ZiggyZag](https://github.com/PascalAI2024/ZiggyZag) · [PAL](https://github.com/PascalAI2024/pal-lang) · [kintunnel](https://github.com/PascalAI2024/kintunnel) |
| 🎮 **Games, 3D & real-time** | Deterministic multiplayer combat, orbital mechanics, persistent galaxy state, browser 3D | [IGD Dev Lab](https://igddev.com) |
| 🔌 **Embedded & hardware** | ESP32-S3 firmware, AMOLED + voice interfaces, guarded tool bridges on a chip the size of a stamp | [JarvisNano](https://github.com/PascalAI2024/JarvisNano) |

**Working stack:** real-time systems (WebSocket, multiplayer, live state sync) ·
AI/ML integration (LLMs, RAG, vector search) · cross-platform (Flutter, Dioxus,
React Native, WASM) · full-stack TypeScript (Next.js, NestJS, Prisma, tRPC) ·
systems programming (Rust, Go, Zig, C) · Elixir/Phoenix · Python ·
infrastructure (Docker, Traefik, CI/CD, Dokploy).

---

## The house platform

The studio runs on tooling we built for ourselves. It's source-private, so it
appears here as capability, not as proof — the shapes are public, the machinery
isn't.

| System | What it does | Public state |
| :-- | :-- | :-- |
| **JarvisMCP** | One Code-Mode MCP gateway that replaces dozens of individual MCP servers with two tools, exposing a company's whole operations surface to agents — safely and with scoped access | Source-private · shape described [here](https://github.com/PascalAI2024/picoarmy) |
| **Overwatch** | The operations console — Bun, TanStack Start, PostgreSQL, Drizzle. Where agent and system activity becomes something a human can actually supervise | Source-private |
| **ButlerCRM** | Client CRM platform on Elixir / Phoenix LiveView, built for follow-up that doesn't get dropped | Source-private · product |
| **GigaBrain** | A reusable knowledge-vault template: an agent-pointable operating memory that ships with structure and *no data* — nothing client-, project-, or person-specific | Source-private · template |
| **Agent sandbox fleet** | Self-hosted, disposable environments so agents can run real work without touching anything that matters | Source-private |

What never gets published: client data, credentials, production topology,
security controls, internal prompts, automation recipes, or access paths. The
[public boundaries](https://github.com/PascalAI2024/portfolio/blob/main/PUBLIC_BOUNDARIES.md)
are written down so the line isn't improvised.

---

## The receipts

Anyone can write "high performance." Here's the version with links attached.

| Result | What it actually means | Open it |
| :-- | :-- | :-- |
| **52 → 377 tok/s** | Generation speedup on a 20B‑A1B ternary MoE, from local CUDA patches | [Maple CUDA](https://github.com/PascalAI2024/maple-preview-windows-cuda) |
| **1,457 → 10,674 tok/s** | Prompt processing, measured in a fresh A/B/B/A run — not one lucky pass | [benchmark data](https://huggingface.co/datasets/x0me/maple-preview-cuda-benchmarks) |
| **103 / 103** | Every enabled build passed the full CPU‑reference correctness matrix. Speed without a correctness gate isn't a result | [method](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/maple-cuda.md) |
| **7.3 GB VRAM** | A 20B model made practical on a 16 GB consumer card instead of datacenter hardware | [repo](https://github.com/PascalAI2024/maple-preview-windows-cuda) |
| **Frozen forecasts** | Predictions committed *before* each deadline, then graded against official actuals by automation | [fplbench board](https://huggingface.co/spaces/x0me/fplbench-board) |
| **A corrections log** | A public record of what I got wrong, filed next to what I got right | [evidence ledger](https://github.com/PascalAI2024/portfolio/blob/main/proof/README.md) |

---

## Flagships

<table>
<tr>
<td width="50%" valign="top">

### 🧪 [fplbench](https://github.com/PascalAI2024/fplbench)

**Applied ML that keeps score.**

A leakage-safe Fantasy Premier League dataset and forecasting system. The
forecast is committed before the deadline, the model plays its own public team,
and automation grades the frozen forecast after the gameweek. Source, validation
artifacts, a Hugging Face dataset, a living board, and an explicit corrections
trail. It is very hard to fool a benchmark that grades you in public.

`Python` · [dataset](https://huggingface.co/datasets/x0me/fplbench) · [live board](https://huggingface.co/spaces/x0me/fplbench-board) · [case study](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/fplbench.md)

</td>
<td width="50%" valign="top">

### ⚡ [Maple CUDA](https://github.com/PascalAI2024/maple-preview-windows-cuda)

**Performance with correctness gates.**

Seven local CUDA patches made a 20B‑A1B ternary model practical on a 16 GB GPU
under Windows. The repo records the dead ends as well as the wins: generation
52 → 377 tok/s, prompt processing 1,457 → 10,674 tok/s, and a 103-case
CPU-reference matrix every enabled build had to clear before it counted.

`CUDA` · `PowerShell` · [benchmarks](https://huggingface.co/datasets/x0me/maple-preview-cuda-benchmarks) · [case study](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/maple-cuda.md)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🐚 [ZiggyZag](https://github.com/PascalAI2024/ZiggyZag)

**Native software with an approval boundary.**

An all-Zig shell workspace: a readable shell core, native Windows and macOS
terminal hosts, a cross-platform launcher, and a local AI sidecar. The agent
proposes mutations; the host owns the approval. Process boundaries, release
artifacts, platform caveats, and conformance tests are all exposed rather than
hidden behind a pretty screenshot.

`Zig` · [releases](https://github.com/PascalAI2024/ZiggyZag/releases) · [case study](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/ziggyzag.md)

</td>
<td width="50%" valign="top">

### 🤖 [JarvisNano](https://github.com/PascalAI2024/JarvisNano)

**Where AI stops being a chat box.**

ESP32-S3 firmware for a pocket desktop assistant: round AMOLED display, touch,
microphone and speaker paths, live voice, device diagnostics, and a guarded tool
bridge. The v1 target is real hardware sitting on a real desk — and the
unfinished tracks stay labeled unfinished.

`C` · `ESP-IDF` · [architecture](https://github.com/PascalAI2024/JarvisNano/blob/main/docs/ARCHITECTURE.md) · [case study](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/jarvisnano.md)

</td>
</tr>
</table>

---

## Everything public, with its honest status

No inflation. Status labels are the conservative ones from the
[public project index](https://github.com/PascalAI2024/portfolio/blob/main/docs/PUBLIC_PROJECT_INDEX.md).

| Project | Lane | Where it actually stands |
| :-- | :-- | :-- |
| [fplbench](https://github.com/PascalAI2024/fplbench) | Applied ML / data | Live 2026/27 benchmark — dataset, Space, frozen predictions, automated scoring |
| [Maple CUDA](https://github.com/PascalAI2024/maple-preview-windows-cuda) | GPU performance | v1.0 release plus post-release MMQ research; raw logs and CPU-reference matrix public |
| [Qwen Quant Bench](https://github.com/PascalAI2024/qwen38-27b-quant-bench) | LLM research | Completed research record — recipes, harnesses, raw results, corrections log |
| [ZiggyZag](https://github.com/PascalAI2024/ZiggyZag) | Native dev tools | **Active alpha.** Check current CI before you adopt it |
| [JarvisNano](https://github.com/PascalAI2024/JarvisNano) | Embedded AI | Hardware release candidate — not a finished consumer product |
| [VibeGotchi](https://github.com/PascalAI2024/VibeGotchi) | Web product | [Live](https://vibegotchi.pages.dev) — read-only OAuth, documented permission model |
| [PicoArmy](https://github.com/PascalAI2024/picoarmy) | Agent fleets | Public prototype — Postgres/RLS model, MCP scopes, audit paths. No public deployment claimed |
| [Verrow](https://github.com/PascalAI2024/verrow) | Data operations | Public prototype — ingestion and mapping done, later surfaces staged |
| [KinTunnel](https://github.com/PascalAI2024/kintunnel) | Self-hosted networking | Runnable MVP, dry-run by default; held back pending dependency-security cleanup |
| [Kaggle Field Notes](https://github.com/PascalAI2024/Kaggle-Portfolio) | Competitive ML | Evidence framework; the result inventory is deliberately incomplete |
| [PAL](https://github.com/PascalAI2024/pal-lang) | Language research | Early concept. A statement of intent, not a finished system |

Forks and source-private repos are never presented as original public proof.
Stars are a nice signal; they are not evidence.

---

## Out of the Dev Lab

Products built at [IGD Dev Lab](https://igddev.com) — the studio's own bets,
deployed across production domains.

**Oxide Studio** unified AI dev environment driving 700+ models · **Juba**
investigative dossier builder with a force-directed knowledge graph ·
**NexusDialer** enterprise contact center with BYOS · **ZeroChat** open-source
voice agent that runs entirely on-device · **DataAlchemy** intelligent column
mapping and automated data workflows · **TariffSync** HTS classification for
auto-parts imports · **VocalFrame** text to talking-head video · **ZeroInbox**
gamified email client · **CallCue** privacy-first calling · **GlowClient**
salon & spa management · **HVAC Recruit** EPA-certified technician staffing ·
**HerCircle** personal safety app · plus a real-time **space strategy game**
with deterministic combat and orbital mechanics.

---

## The range, as a picture

```mermaid
flowchart TB
    P([Somebody has a real problem]) --> W[Web, commerce and content]
    P --> C[CRM, comms and automation]
    P --> A[Agents and AI infrastructure]
    P --> R[Measured research]
    P --> S[Native and systems]
    P --> G[Games, 3D and real-time]
    P --> H[Embedded and hardware]

    W --> CL{{Source-private<br/>running in production}}
    C --> CL
    G --> CL
    A --> PA(PicoArmy)
    A --> ZZ(ZiggyZag)
    R --> F(fplbench)
    R --> Q(Qwen quant study)
    R --> M(Maple CUDA)
    S --> PL(PAL)
    S --> KT(kintunnel)
    H --> J(JarvisNano)
    A --> VG(VibeGotchi)

    PA --> E{{Public artifact<br/>or an explicit limitation}}
    ZZ --> E
    F --> E
    Q --> E
    M --> E
    PL --> E
    KT --> E
    VG --> E
    J --> E
    CL --> B[Boundary stated,<br/>never embellished]
```

---

## How I judge my own work

1. **The artifact must be inspectable.** Source, a live surface, raw evidence, or a clearly bounded public-safe write-up.
2. **The comparison must be fair.** Frozen forecasts, controlled A/B runs, common masks, correctness references, disclosed constraints.
3. **The human boundary must be legible.** Approval, privacy, credentials, and irreversible actions are product decisions — not footnotes.
4. **Status travels with the claim.** A prototype does not get promoted to production by adjective.

More on the method: [capability map](https://github.com/PascalAI2024/portfolio/blob/main/capabilities/README.md) ·
[system shapes](https://github.com/PascalAI2024/portfolio/blob/main/architecture/README.md) ·
[case studies](https://github.com/PascalAI2024/portfolio/blob/main/case-studies/README.md) ·
[evidence ledger](https://github.com/PascalAI2024/portfolio/blob/main/proof/README.md)

---

## Also true

- Half my infrastructure is named after a fictional butler. I've made peace with this.
- A Zig shell, a Roblox scene and a CUDA kernel can land in the same week of commits. This is a feature.
- I keep a public corrections log, which is the least flattering and most useful page I maintain.
- The stack runs from `Shopify Liquid` to `ESP-IDF`. Nobody planned that. It just kept being the right tool.

---

## Work together

The best fit is work that needs product judgment *and* engineering depth: AI and
automation, agent infrastructure, custom software, performance work, research
systems, and ambitious prototypes that have to become maintainable products.

Or, honestly — a website and a CRM that finally talk to each other. That counts too.

<p align="center">
  <a href="https://ingeniousdigital.com/contact"><b>Start a conversation with Ingenious Digital →</b></a><br>
  <sub>Fort Lauderdale, on Eastern time · shipping worldwide</sub>
</p>

<p align="center">
  <sub>
    <a href="https://ingeniousdigital.com">ingeniousdigital.com</a> ·
    <a href="https://igddev.com">igddev.com</a> ·
    <a href="https://huggingface.co/x0me">huggingface.co/x0me</a> ·
    <a href="https://github.com/PascalAI2024/portfolio">the full record</a>
  </sub>
</p>

<!--
  Still reading the source? Then you already pass rule 1.
  The evidence ledger is where the honest version lives:
  https://github.com/PascalAI2024/portfolio/blob/main/proof/README.md
-->

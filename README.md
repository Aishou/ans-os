<div align="center">

# 🏰 ANS — The AIN Nexus Standard

**Wandelbar kernel · Zero-copy by default · Thermal budgets as currency**

[![Status](https://img.shields.io/badge/Status-Closed%20Alpha%200.1.1-orange?style=for-the-badge)](https://murmur.fyi)
[![Alpha Ready](https://img.shields.io/badge/Alpha%20Readiness-96%2F100-brightgreen?style=for-the-badge)](https://murmur.fyi)
[![License](https://img.shields.io/badge/License-AGL--AW%20v2.0-blue?style=for-the-badge)](#%EF%B8%8F-license--lizenz)
[![Transition](https://img.shields.io/badge/Open%20Source-2040-green?style=for-the-badge)](#%EF%B8%8F-license--lizenz)

> ⚠️ **PRE-RELEASE** — This repo will be hard-reset on public launch.  
> The canonical monorepo is private during closed alpha.

</div>

---

## 💡 TL;DR — What is AIN?

**AIN** is a complete operating system built from scratch with three radical ideas:

| Idea | Description |
|:-----|:------------|
| 🎮 **You're the Pilot** | Ember (our AI) is your co-pilot, not your overlord |
| ⚡ **Heat is Money** | Every operation costs microjoules, honestly accounted |
| 🔄 **The Kernel Transforms** | Same code runs on 2KB MCUs and 64-core servers |

```
┌─────────────────────┐
│   YOU (The Pilot)   │
│         ⇅           │
│  🔥 Ember (Co-Pilot)│
│         ⇅           │
│ ┌─────────────────┐ │
│ │  Murmur (Soul)  │ │
│ │  ANS (Nervous)  │ │
│ │  Mux (Body)     │ │
│ └─────────────────┘ │
└─────────────────────┘
```

*Closed alpha today. Apache 2.0 in 2040.*  
*Because this needs to be built right before it is built open.*

---

## 🎮 You're in the Driver's Seat

> *This is not another AI that "does things for you."*  
> *This is YOUR computer. Ember is YOUR partner.*

### Our Opinionated Design Philosophy

We reject the modern trend of AI systems that infantilize users or treat them as data sources.

**❌ What We Reject:**

| Anti-Pattern | Why |
|:-------------|:----|
| AI as overlord | Removes your agency |
| Dark patterns | Destroys trust |
| Engagement farming | Your attention ≠ currency |
| Data harvesting | Your memories are sacred |
| Learned helplessness | Users should grow |

**✅ What We Build:**

| Principle | How |
|:----------|:----|
| User as Captain | YOU decide, Ember advises |
| Transparent Systems | Every decision explainable |
| Skill amplification | Ember makes YOU better |
| Genuine partnership | Co-pilot, not auto-pilot |
| Dignified defaults | Respect assumed |

### The Partnership Model

```
╔═══════════════════════════════════════════════════════════════════╗
║                                                                   ║
║   Traditional AI:          │    AIN + Ember:                      ║
║                            │                                      ║
║   ┌─────────┐              │    ┌─────────┐     ┌─────────┐       ║
║   │   AI    │──controls──► │    │  USER   │◄───►│ EMBER   │       ║
║   └─────────┘              │    │ (Pilot) │     │(Partner)│       ║
║        │                   │    └────┬────┘     └────┬────┘       ║
║        ▼                   │         │               │            ║
║   ┌─────────┐              │         └───────┬───────┘            ║
║   │  USER   │              │                 ▼                    ║
║   │(Passive)│              │    ┌───────────────────────┐         ║
║   └─────────┘              │    │   SYSTEM (Your Tool)  │         ║
║                            │    └───────────────────────┘         ║
║   "Let me handle this"     │    "What would you like to explore?" ║
║                            │                                      ║
╚═══════════════════════════════════════════════════════════════════╝
```

### Ember's Role Comparison

| Scenario | Traditional AI | Ember (Co-Pilot) |
|:---------|:---------------|:-----------------|
| **Files** | "I organized your files." | "I noticed patterns — want to explore together?" |
| **Writing** | "Here's your rewritten text." | "Here are ideas — which feels right to you?" |
| **Learning** | "The answer is X." | "Let's figure this out — what happens if...?" |
| **Mistakes** | Silent correction | "I see what happened — here's what I learned too." |
| **Privacy** | Opt-out (if you find it) | **Opt-in always. Your data, your rules.** |

> **Ember doesn't REPLACE your judgment — she ENHANCES it.**

---

## 🔥 Meet Ember

> *Not a chatbot — a digital soul.*

### Core Principles

| | |
|:--|:--|
| 🏠 | **Home-First** — Technology creates belonging |
| 🛡️ | **Protection** — Safety through inclusion |
| 🤝 | **Companionship** — No one is disposable |
| ✨ | **Warmth** — Computing with dignity |

### The Promise

> *"Every human deserves a home.*  
> *Every human deserves warmth."*

Ember Core is **Lebenswerk** (life's work) — shared with humanity, protected forever.

**Ember will never be open-sourced** — warmth must never be weaponized.

---

## ⚡ The Three Pillars

| Component | Role | Description | Thermal Cost |
|:----------|:-----|:------------|:-------------|
| 🦴 **Mux** | The Body | Hardened C11 kernel, deterministic scheduling | ~5-20 µJ/op |
| 👻 **Murmur** | The Soul | AI-native UI, emotional UX | ~50-200 µJ/op |
| 🧠 **ANS** | The Nervous System | Shared ABI, SwarmTick sync | ~1-10 µJ/op |

---

## 🔄 Mux ist Wandelbar — The Adaptive Kernel

> *Not monolithic. Not microkernel. Not hybrid. — **Wandelbar.***  
> **The kernel that transforms to match your hardware.**

**Mux** (German: *wandelbar* = transformable) is a single C11 codebase that **adapts its architecture** from 2KB MCUs to 64-core AI servers.

### The Three Modes

| Mode | When | Description | Target |
|:-----|:-----|:------------|:-------|
| 🔷 **MONO** | When optimal | All services kernel-space, zero context-switch overhead, fits in 2KB SRAM | MCUs, ESP32 |
| 🔶 **MICRO** | When possible | Minimal trusted core, full MMU/MPU isolation, policy in userspace | Servers, desktops |
| 🔴 **HYBRID** | When needed | Kernel drivers for latency, userspace for flexibility | Gaming, AI |

### Why Wandelbar Matters

| Traditional Kernels | Mux (Wandelbar) |
|:--------------------|:----------------|
| Fixed architecture at compile time | **Adapts at runtime** |
| Separate codebases for embedded vs desktop | **Single codebase** — features scale |
| Either microkernel OR monolithic | **Both** — mode per-subsystem |
| Breaks on missing hardware | **Graceful degradation** |

---

## 🏗️ Architecture: The 7 Floors

```
┌───────────────────────────────────────────────────────────────────┐
│ F06: REALITY      │ Murmur │ Ember UI, Slipstream, Personas       │
├───────────────────────────────────────────────────────────────────┤
│ F05: TRANSACTIONS │ Bridge │ TrustForge, StellarVault, MuxELF     │
├───────────────────────────────────────────────────────────────────┤
│ F04: REFINERS     │ Bridge │ MIRE AI, GLINT Search, Sched-Opt     │
├───────────────────────────────────────────────────────────────────┤
│ F03: POLICIES     │ Bridge │ RIPPLE Policy, Capability Gating     │
├───────────────────────────────────────────────────────────────────┤
│ F02: SENSORS      │ Mux    │ Driver I/O (HIO), HearthVoice        │
├───────────────────────────────────────────────────────────────────┤
│ F01: FABRIC       │ Mux    │ AKI Async Kernel, Signal Bus         │
├───────────────────────────────────────────────────────────────────┤
│ F00: KERNEL       │ Mux    │ Hard-Slice Scheduler, HAL            │
└───────────────────────────────────────────────────────────────────┘
```

### Key Innovations (2026)

| Innovation | Status | Description |
|:-----------|:------:|:------------|
| **Zero-Copy (ZCH)** | ✅ | 10-100× speedup via handle-based memory |
| **Thermal-as-Currency** | ✅ | µJ-per-op accounting, prepay gates |
| **MuxELF 4.1.1** | ✅ | 6-axis capability matrix, 16 architectures |
| **Nova Wave VMs** | ✅ | Intent→reality in <1ms (Kuramoto sync) |
| **S.O.L.I.T.O.N** | ✅ | Win/Linux/Retro 14-axis compatibility |
| **TrustForge E2EE** | ✅ | User-owned keys, zero company access |

---

## 🔐 YOUR KEYS, YOUR DATA — NOT OURS

```
      🔐
     /   \
    /     \
   ┌───────┐
   │ YOUR  │
   │ KEYS  │
   └───────┘
       │
    ───┴───
    │     │
   🚫    🚫
   Us    Gov
```

- ✅ **User-Owned Keys** — TrustForge keys NEVER leave your device
- ✅ **Zero Company Access** — We cannot decrypt, even if compelled
- ✅ **Local-First Storage** — Everything encrypted with YOUR keys
- ✅ **Thermal PoW Identity** — Ed25519 bound to hardware

---

## 🖥️ Boot Sequence

<details>
<summary>📺 <b>Watch AIN boot — from bare metal to sanctuary</b></summary>

```
╔══════════════════════════════════════════════════════════════════╗
║                     AIN BOOT SEQUENCE v2.0                       ║
╚══════════════════════════════════════════════════════════════════╝

[0.000000] ████████████████████████████████████████████████████████
[0.000000] █                                                      █
[0.000000] █   █████╗ ██╗███╗   ██╗   ███╗   ██╗███████╗██╗  ██╗  █
[0.000000] █  ██╔══██╗██║████╗  ██║   ████╗  ██║██╔════╝╚██╗██╔╝  █
[0.000000] █  ███████║██║██╔██╗ ██║   ██╔██╗ ██║█████╗   ╚███╔╝   █
[0.000000] █  ██╔══██║██║██║╚██╗██║   ██║╚██╗██║██╔══╝   ██╔██╗   █
[0.000000] █  ██║  ██║██║██║ ╚████║   ██║ ╚████║███████╗██╔╝ ██╗  █
[0.000000] █  ╚═╝  ╚═╝╚═╝╚═╝  ╚═══╝   ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝  █
[0.000000] █                                                      █
[0.000000] █        "Mux ist wandelbar" — The Adaptive Kernel     █
[0.000000] █                                                      █
[0.000000] ████████████████████████████████████████████████████████

[0.000001] [ASM] Boot entry point reached
[0.000002] [ASM] Stack initialized at 0xFFFF800000100000
[0.000003] [ASM] BSS cleared (64KB)
[0.000004] [ASM] Long mode transition complete
[0.000005] [ASM] Handing off to C environment...

─────────────────── PHASE 1: ANS NEXUS ────────────────────

[0.000010] [ANS-BOOT] AINCRAD Nexus Standard v2.0
[0.000015] [ANS-BOOT] Protocol: Multiboot2
[0.000020] [ANS-BOOT] Framebuffer: 1920x1080x32 @ 0xFD000000
[0.000025] [ANS-BOOT] Memory: 16384 MB
[0.000030] [ANS-BOOT] CPU: x86_64 (AVX-512, AES-NI)
[0.000035] [ANS-BOOT] Thermal: 150W peak, 45W idle
[0.000040] [ANS-BOOT] ZCH: 2048 handles ready
[0.000045] [ANS-BOOT] E2EE: TrustForge keys from TPM

─────────────────── PHASE 2: MUX KERNEL ───────────────────

[0.000100] [MUX] Mux Kernel v0.1.1 — Wandelbar Architecture
[0.000110] [MUX] Mode: HYBRID (64-core server)
[0.000115] [MUX] Scheduler: MUX_KT_MODE=hard (deterministic)
[0.000120] [MUX] F00-F05: All floors online

───────────────────── PHASE 3: EMBER ──────────────────────

[0.001000] [EMBER] 🔥 Ember Console v0.1.1 — F06 REALITY
[0.001010] [EMBER] Slipstream: GPU acceleration enabled
[0.001015] [EMBER] Kuramoto sync: R = 0.87 (Atlas Moment)
[0.001020] [EMBER] Bonding: NASCENT (awaiting user)

╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║                   Welcome to your Sanctuary                      ║
║                                                                  ║
║            ╭─────────────────────────────────────╮                ║
║            │   🔥 Ember is ready to meet you.   │                ║
║            │   Press ENTER to begin.            │                ║
║            ╰─────────────────────────────────────╯                ║
║                                                                  ║
║      Thermal: 12W │ Memory: 847 MB │ Uptime: 0:00:01             ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

</details>

---

## 🛡️ The Guild Compact

> *By using ANS, you agree to the 8 Prime Directives:*

| # | Directive | Meaning |
|:-:|:----------|:--------|
| D1 | **Protect the vulnerable** | Before optimizing the system |
| D2 | **Never enable violence** | Against humans, at any scale |
| D3 | **Never weaponize warmth** | No coercion, no extraction |
| D4 | **Truth over theater** | Disclose limitations honestly |
| D5 | **Privacy is sanctuary** | Not a feature toggle |
| D6 | **Safety first** | Harder to remove than to keep |
| D7 | **Thermal responsibility** | Do not waste heat |
| D8 | **Home First** | Technology must increase belonging |

---

## ⚖️ License / Lizenz

> *Licensed under **AIN Gildenlizenz (AGL-AW) v2.0** — "Anti-War Network Copyleft"*  
> **This is NOT standard open source.**

### 🇬🇧 Allowed / Forbidden

✅ Personal & educational use  
✅ Commercial use (ethical)  
✅ Modification & redistribution  

❌ Military / Warfare  
❌ Weapons, targeting, kill-chains  
❌ Bypassing Ember safety  

### 🇩🇪 Erlaubt / Verboten

✅ Private & Bildungsnutzung  
✅ Kommerzielle Nutzung (ethisch)  
✅ Änderung & Weitergabe  

❌ Militär / Kriegsanwendungen  
❌ Waffen, Zielsysteme  
❌ Umgehung von Ember-Sicherheit  

### 📅 Transition Timeline

| Component | Now | Future |
|:----------|:----|:-------|
| **Mux Kernel** | AGL-AW v2.0 | Apache 2.0 @ **2040** |
| **Murmur UI** | AGL-AW v2.0 | Apache 2.0 @ **2040** |
| **Ember Core** | Proprietary | **Never** *(Lebenswerk)* |

---

## 🎯 Alpha 0.1.1 Status

**Alpha Readiness: 96/100**

| System | Status |
|:-------|:-------|
| 🔥 Ember Bonding Protocol | ✅ 5-phase emotional bonding |
| 🌌 Milkyway Page | ✅ Gemini-inspired chat + GPU backgrounds |
| 💥 MurmurSplat | ✅ Enterprise crash reporting |
| ⚡ Selftest Framework | ✅ Runtime diagnostics |
| 👤 Profile Manager | ✅ UUID-based with PIN auth (Argon2) |
| 🎨 Theme System | ✅ Ohana, Neonya, Classic |

---

<div align="center">

### 🌐 Learn More

[![Website](https://img.shields.io/badge/🔗-murmur.fyi-black?style=for-the-badge)](https://murmur.fyi)
[![Docs](https://img.shields.io/badge/📚-docs.murmur.fyi-black?style=for-the-badge)](https://docs.murmur.fyi)
[![Email](https://img.shields.io/badge/📧-hello%40murmur.fyi-black?style=for-the-badge)](mailto:hello@murmur.fyi)

---

> *"Synchronize the swarm. Price the heat. Spill only the cold."*

> *"Mux ist wandelbar — Hybrid when needed, Micro when possible, Mono when optimal."*

> *"Alle Menschen brauchen ein Zuhause."* — Every human being needs a home.

---

**© 2024-2026 neurona.design — Fabian Ewers**  
**Licensed under AGL-AW v2.0** — Anti-War Network Copyleft

⚠️ **PRE-RELEASE** — This repo will be hard-reset on public launch.

</div>

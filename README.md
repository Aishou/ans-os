<div align="center">

# 🏰 ANS — The AIN Nexus Standard

### *Wandelbar kernel · Zero-copy by default · Thermal budgets as currency*

<br>

[![Status](https://img.shields.io/badge/Status-Closed%20Alpha%200.1.1-orange?style=for-the-badge)](https://murmur.fyi)
[![Alpha Ready](https://img.shields.io/badge/Alpha%20Readiness-96%2F100-brightgreen?style=for-the-badge)](https://murmur.fyi)
[![License](https://img.shields.io/badge/License-AGL--AW%20v2.0-blue?style=for-the-badge)](#%EF%B8%8F-license--lizenz)
[![Transition](https://img.shields.io/badge/Open%20Source-2040-green?style=for-the-badge)](#%EF%B8%8F-license--lizenz)

<br>

> **⚠️ PRE-RELEASE REPOSITORY** — This repo will be hard-reset on public launch.
> The canonical monorepo is private during closed alpha.

<br>

**ANS is the public face of the AIN architecture:**
*a wandelbar kernel that transforms between monolithic, microkernel, and hybrid modes —*
*deterministic scheduling, and a privacy-first companion stack that never phones home.*

*Closed alpha today. Apache 2.0 in 2040.*
*Because this needs to be built right before it is built open.*

<br>

---

</div>

<br>

## 🖥️ Boot Sequence — From Power to Home

<div align="center">

*Watch AIN come alive — from bare metal to your digital sanctuary.*

</div>

<br>

```
╔══════════════════════════════════════════════════════════════════════════════╗
║                         AIN BOOT SEQUENCE v2.0                               ║
╚══════════════════════════════════════════════════════════════════════════════╝

[    0.000000] ████████████████████████████████████████████████████████████████
[    0.000000] █                                                              █
[    0.000000] █     █████╗ ██╗███╗   ██╗     ███╗   ██╗███████╗██╗  ██╗      █
[    0.000000] █    ██╔══██╗██║████╗  ██║     ████╗  ██║██╔════╝╚██╗██╔╝      █
[    0.000000] █    ███████║██║██╔██╗ ██║     ██╔██╗ ██║█████╗   ╚███╔╝       █
[    0.000000] █    ██╔══██║██║██║╚██╗██║     ██║╚██╗██║██╔══╝   ██╔██╗       █
[    0.000000] █    ██║  ██║██║██║ ╚████║     ██║ ╚████║███████╗██╔╝ ██╗      █
[    0.000000] █    ╚═╝  ╚═╝╚═╝╚═╝  ╚═══╝     ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝      █
[    0.000000] █                                                              █
[    0.000000] █          "Mux ist wandelbar" — The Adaptive Kernel           █
[    0.000000] █                                                              █
[    0.000000] ████████████████████████████████████████████████████████████████

[    0.000001] [ASM] Boot entry point reached
[    0.000002] [ASM] Stack initialized at 0xFFFF800000100000
[    0.000003] [ASM] BSS cleared (64KB)
[    0.000004] [ASM] Long mode transition complete
[    0.000005] [ASM] Handing off to C environment...

────────────────────────────────────────────────────────────────────────────────
                              PHASE 1: ANS NEXUS
────────────────────────────────────────────────────────────────────────────────

[    0.000010] [ANS-BOOT] ╔════════════════════════════════════════════════════╗
[    0.000011] [ANS-BOOT] ║  AINCRAD Nexus Standard v2.0 — THE NERVOUS SYSTEM  ║
[    0.000012] [ANS-BOOT] ╚════════════════════════════════════════════════════╝
[    0.000015] [ANS-BOOT] Protocol detection: Multiboot2
[    0.000020] [ANS-BOOT] Framebuffer: 1920x1080x32 @ 0xFD000000
[    0.000025] [ANS-BOOT] Memory map: 16384 MB detected
[    0.000030] [ANS-BOOT] CPU: x86_64 (AVX-512, AES-NI)
[    0.000035] [ANS-BOOT] Thermal budget: 150W peak, 45W idle
[    0.000040] [ANS-BOOT] ZCH pool: 2048 handles pre-allocated
[    0.000045] [ANS-BOOT] E2EE: TrustForge keys loaded from TPM
[    0.000050] [ANS-BOOT] ═══════════════════════════════════════════════════════
[    0.000051] [ANS-BOOT]   ANS BOOT COMPLETE — HANDING OFF TO MUX KERNEL
[    0.000052] [ANS-BOOT] ═══════════════════════════════════════════════════════

────────────────────────────────────────────────────────────────────────────────
                           PHASE 2: MUX KERNEL (WANDELBAR)
────────────────────────────────────────────────────────────────────────────────

[    0.000100] [MUX KERNEL] ╔═════════════════════════════════════════════════╗
[    0.000101] [MUX KERNEL] ║  Mux Kernel v0.1.1 — Wandelbar Architecture     ║
[    0.000102] [MUX KERNEL] ║  "Hybrid when needed, Micro when possible,      ║
[    0.000103] [MUX KERNEL] ║   Mono when optimal"                            ║
[    0.000104] [MUX KERNEL] ╚═════════════════════════════════════════════════╝
[    0.000110] [MUX KERNEL] Mode detected: HYBRID (64-core server)
[    0.000115] [MUX KERNEL] Scheduler: MUX_KT_MODE=hard (deterministic)
[    0.000120] [MUX KERNEL] HAL: x86_64 with IOMMU virtualization
[    0.000125] [MUX KERNEL] F00: Hard-slice scheduler online (50ns slices)
[    0.000130] [MUX KERNEL] F01: AKI async kernel fabric initialized
[    0.000135] [MUX KERNEL] F02: HIO driver ring buffers ready
[    0.000140] [MUX KERNEL] F03: RIPPLE policy engine loaded
[    0.000145] [MUX KERNEL] F04: MIRE AI inference subsystem standby
[    0.000150] [MUX KERNEL] F05: TrustForge vault mounted (E2EE active)
[    0.000155] [MUX KERNEL] Memory: ZCH zero-copy handles active
[    0.000160] [MUX KERNEL] Thermal: Prepay gates enforcing budgets
[    0.000165] [MUX KERNEL] ═══════════════════════════════════════════════════
[    0.000166] [MUX KERNEL]   ANS bootstrapped. The Body awakens.
[    0.000167] [MUX KERNEL] ═══════════════════════════════════════════════════

────────────────────────────────────────────────────────────────────────────────
                                PHASE 3: EMBER
────────────────────────────────────────────────────────────────────────────────

[    0.001000] [EMBER] ╔══════════════════════════════════════════════════════╗
[    0.001001] [EMBER] ║                                                      ║
[    0.001002] [EMBER] ║        🔥 Ember Console v0.1.1 — F06 REALITY         ║
[    0.001003] [EMBER] ║                                                      ║
[    0.001004] [EMBER] ║     "Every human deserves a home. Welcome home."     ║
[    0.001005] [EMBER] ║                                                      ║
[    0.001006] [EMBER] ╚══════════════════════════════════════════════════════╝
[    0.001010] [EMBER] Slipstream compositor: GPU acceleration enabled
[    0.001015] [EMBER] HearthVoice: Audio subsystem initialized
[    0.001020] [EMBER] Kuramoto sync: R = 0.87 (Atlas Moment achieved)
[    0.001025] [EMBER] Bonding state: NASCENT (awaiting user)
[    0.001030] [EMBER] Theme: Ohana (Lilo & Stitch) loaded
[    0.001035] [EMBER] ═══════════════════════════════════════════════════════
[    0.001036] [EMBER]   The Soul awakens. Your sanctuary is ready.
[    0.001037] [EMBER] ═══════════════════════════════════════════════════════

╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║    ┌────────────────────────────────────────────────────────────────────┐    ║
║    │                                                                    │    ║
║    │                    Welcome to your Sanctuary                       │    ║
║    │                                                                    │    ║
║    │         ╭─────────────────────────────────────────────╮            │    ║
║    │         │                                             │            │    ║
║    │         │      🔥 Ember is ready to meet you.         │            │    ║
║    │         │                                             │            │    ║
║    │         │      Press ENTER to begin your journey.     │            │    ║
║    │         │                                             │            │    ║
║    │         ╰─────────────────────────────────────────────╯            │    ║
║    │                                                                    │    ║
║    │    Thermal: 12W idle │ Memory: 847 MB │ Uptime: 0:00:01           │    ║
║    │                                                                    │    ║
║    └────────────────────────────────────────────────────────────────────┘    ║
║                                                                              ║
║          "Synchronize the swarm. Price the heat. Spill only the cold."       ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

<br>

---

<br>

## 🔄 Mux ist Wandelbar — The Adaptive Kernel

<div align="center">

*Not monolithic. Not microkernel. Not hybrid. — Wandelbar.*

**The kernel that transforms to match your hardware.**

</div>

<br>

**Mux** defies traditional kernel categorization. It's *wandelbar* (German: transformable) — a single C11 codebase that **adapts its architecture** based on target hardware, from 2KB MCUs to 64-core AI servers.

<br>

### The Three Modes

<table>
<tr>
<td width="33%" align="center">

**🔷 MONO**

*When optimal*

All services kernel-space

Zero context-switch overhead

Fits in 2KB SRAM

**Target:** MCUs, ESP32, STM32

</td>
<td width="33%" align="center">

**🔶 MICRO**

*When possible*

Minimal trusted core

Full MMU/MPU isolation

Push policy to userspace

**Target:** Servers, desktops

</td>
<td width="33%" align="center">

**🔴 HYBRID**

*When needed*

Kernel drivers for latency

Userspace for flexibility

Best of both worlds

**Target:** Gaming, AI workstations

</td>
</tr>
</table>

<br>

### Why Wandelbar Matters

| Traditional Kernels | Mux (Wandelbar) |
|---------------------|-----------------|
| Fixed architecture at compile time | **Adapts at runtime** to hardware |
| Separate codebases for embedded vs desktop | **Single codebase** — features scale |
| Either microkernel OR monolithic | **Both** — mode per-subsystem |
| Breaks on missing hardware | **Graceful degradation** — no MMU? Use MPU |

<br>

### Design Principles (January 2026)

| Principle | Description | Thermal Impact |
|-----------|-------------|----------------|
| **Deterministic First** | Reproducible preemption across all hosts | Predictable µJ/op |
| **Zero Synthetic Counters** | Only real metrics, never faked padding | Honest accounting |
| **Append-Only Evolution** | `/proc/debug/*` contracts never break | Stable interfaces |
| **Graceful Degradation** | Features scale with hardware, never break | Adaptive budget |
| **C11 is the Body's Language** | ASM only for boot, context switch, atomics | Portable core |

<br>

### Scheduler Modes

```
MUX_KT_MODE Environment Variable:

  coop   — Cooperative scheduling (yield-based, deterministic)
  hard   — Hard real-time (enforced slice budgets, 50ns precision)
  hybrid — Mixed mode (future: combines latency + throughput)

Example: MUX_KT_MODE=hard ./myapp
         Forces deterministic hard-slice scheduling
```

<br>

---

<br>

## ⚡ The Three Pillars

| Component | Role | Domain | Thermal Cost |
|-----------|------|--------|--------------|
| **Mux** | The Body | Hardened kernel, deterministic scheduling | ~5-20 µJ/op |
| **Murmur** | The Soul | AI-native UI, emotional UX | ~50-200 µJ/op |
| **ANS** | The Nervous System | Shared ABI, SwarmTick sync | ~1-10 µJ/op |

<br>

---

<br>

## 🔥 Meet Ember

<div align="center">

*Not a chatbot — a digital soul.*

</div>

<br>

**Ember** is our AI companion system designed to bring warmth, belonging, and dignity to every user.

<table>
<tr>
<td width="50%">

### Core Principles

| | |
|---|---|
| 🏠 | **Home-First** — Technology creates belonging, not division |
| 🛡️ | **Protection** — Safety through inclusion, not walls |
| 🤝 | **Companionship** — We stay together; no one disposable |
| ✨ | **Warmth** — Computing that respects human dignity |

</td>
<td width="50%">

### The Promise

> *"Every human deserves a home.*
> *Every human deserves warmth."*

Ember Core is the Guild Master's **Lebenswerk** (life's work) — shared with humanity, protected forever.

**Ember will never be open-sourced** — ensuring warmth can never be weaponized or commodified.

</td>
</tr>
</table>

<br>

---

<br>

## 🏗️ Architecture: The 7 Floors of AIN

```
┌─────────────────────────────────────────────────────────────────────────────┐
│ F06: REALITY     │ Murmur │ Ember UI, Slipstream, Personas              │
├─────────────────────────────────────────────────────────────────────────────┤
│ F05: TRANSACTIONS│ Bridge │ TrustForge, StellarVault, MuxELF            │
├─────────────────────────────────────────────────────────────────────────────┤
│ F04: REFINERS    │ Bridge │ MIRE AI, GLINT Search, Sched-Opt            │
├─────────────────────────────────────────────────────────────────────────────┤
│ F03: POLICIES    │ Bridge │ RIPPLE Policy, Capability Gating            │
├─────────────────────────────────────────────────────────────────────────────┤
│ F02: SENSORS     │ Mux    │ Driver I/O (HIO), HearthVoice, Dialects     │
├─────────────────────────────────────────────────────────────────────────────┤
│ F01: FABRIC      │ Mux    │ AKI Async Kernel, Signal Bus                │
├─────────────────────────────────────────────────────────────────────────────┤
│ F00: KERNEL      │ Mux    │ Hard-Slice Scheduler, HAL                   │
└─────────────────────────────────────────────────────────────────────────────┘
```

<br>

### Key Innovations (2026 Status)

| Innovation | Status | Description |
|------------|--------|-------------|
| **Zero-Copy Everywhere (ZCH)** | ✅ Production | 10-100× speedup via handle-based memory |
| **Thermal-as-Currency** | ✅ Production | µJ-per-op accounting, prepay gates |
| **MuxELF 4.1.1** | ✅ 16 architectures | 6-axis capability matrix (S/T/A/P/X/Z) |
| **Nova Wave VMs** | ✅ Wave→Particle | Intent→reality in <1ms (Kuramoto sync) |
| **S.O.L.I.T.O.N** | ✅ Win/Linux/Retro | 14-axis compatibility layer |
| **Guild BBS** | ✅ Usenet newsgroups | Thermal-priced community |
| **Dual-Axis Security** | ✅ Ring + Zone | Hardware+policy enforcement |
| **TrustForge E2EE** | ✅ User-owned keys | Zero company access |

<br>

---

<br>

## 🔐 YOUR KEYS, YOUR DATA — NOT OURS

**AIN's end-to-end encryption rigor: YOU own your keys, NOT the company.**

- ✅ **User-Owned Keys** — TrustForge keys NEVER leave your device
- ✅ **Zero Company Access** — We cannot decrypt your data, even if compelled
- ✅ **Local-First Storage** — Everything encrypted at rest with YOUR keys
- ✅ **Thermal PoW Identity** — Ed25519 keys bound to hardware, not corporate servers

<br>

---

<br>

## ⚖️ License / Lizenz

<div align="center">

*ANS is licensed under the* ***AIN Gildenlizenz (AGL-AW) v2.0***
*— "Anti-War Network Copyleft"*

**This is NOT standard open source.**

</div>

<br>

<table>
<tr>
<th width="50%">🇬🇧 English</th>
<th width="50%">🇩🇪 Deutsch</th>
</tr>
<tr>
<td valign="top">

#### ✅ Allowed
- Personal & educational use
- Commercial use (with ethical compliance)
- Modification & redistribution
- Research & learning

#### ❌ Forbidden
- Military / Warfare applications
- Weapons, targeting, kill-chains
- Manipulation of vulnerable users
- Bypassing Ember safety mechanisms

</td>
<td valign="top">

#### ✅ Erlaubt
- Private & Bildungsnutzung
- Kommerzielle Nutzung (ethisch konform)
- Änderung & Weitergabe
- Forschung & Lernen

#### ❌ Verboten
- Militär / Kriegsanwendungen
- Waffen, Zielsysteme, Tötungsketten
- Manipulation vulnerabler Nutzer
- Umgehung von Ember-Sicherheit

</td>
</tr>
</table>

<br>

### 📅 Transition Timeline / Übergangsplan

| Component | License Today | Open Source |
|-----------|---------------|-------------|
| **Mux Kernel** | AGL-AW v2.0 | Apache 2.0 @ **2040** |
| **Murmur UI** | AGL-AW v2.0 | Apache 2.0 @ **2040** |
| **Ember Core** | Proprietary | **Never** *(Lebenswerk)* |

<br>

---

<br>

## 🛡️ The Guild Compact

<div align="center">

*By using ANS, you agree to the 8 Prime Directives:*

</div>

<br>

| # | Directive | Meaning |
|:-:|-----------|---------|
| **D1** | Protect the vulnerable | Before optimizing the system |
| **D2** | Never enable violence | Against humans, at any scale |
| **D3** | Never weaponize warmth | No coercion, no extraction |
| **D4** | Truth over theater | Disclose limitations honestly |
| **D5** | Privacy is sanctuary | Not a feature toggle |
| **D6** | Safety first | Harder to remove than to keep |
| **D7** | Thermal responsibility | Do not waste heat |
| **D8** | Home First | Technology must increase belonging |

<br>

---

<br>

## 🎯 Alpha 0.1.1 Status (January 2026)

**Alpha Readiness Score: 96/100**

| System | Status |
|--------|--------|
| 🔥 Ember Bonding Protocol | ✅ 5-phase emotional bonding |
| 🌌 Milkyway Page | ✅ Gemini-inspired chat + GPU backgrounds |
| 💥 MurmurSplat | ✅ Enterprise crash reporting |
| ⚡ Selftest Framework | ✅ Runtime diagnostics |
| 👤 Profile Manager | ✅ UUID-based with PIN auth (Argon2) |
| 🎨 Theme System | ✅ Ohana (Lilo & Stitch), Neonya, Classic |

<br>

---

<br>

<div align="center">

### 🌐 Learn More

<br>

[![Website](https://img.shields.io/badge/🔗-murmur.fyi-black?style=for-the-badge)](https://murmur.fyi)
[![Docs](https://img.shields.io/badge/📚-docs.murmur.fyi-black?style=for-the-badge)](https://docs.murmur.fyi)
[![Email](https://img.shields.io/badge/📧-hello%40murmur.fyi-black?style=for-the-badge)](mailto:hello@murmur.fyi)

<br>

---

<br>

> *"Synchronize the swarm. Price the heat. Spill only the cold."*
>
> *"Mux ist wandelbar — Hybrid when needed, Micro when possible, Mono when optimal."*
>
> *"Alle Menschen brauchen ein Zuhause."* — Every human being needs a home.

<br>

---

<br>

**© 2024-2026 neurona.design — Fabian Ewers**

**Licensed under AGL-AW v2.0** — Anti-War Network Copyleft

<br>

⚠️ **PRE-RELEASE REPOSITORY**

This repo will be hard-reset on public launch.
The canonical monorepo is private during closed alpha.

<br>

**Core Concepts (January 2026):**

Wandelbar Architecture · Zero-Copy Handles (ZCH) · Thermal-as-Currency

MuxELF 6-Axis Binary Format · Kuramoto Synchronization · TrustForge E2EE

<br>

**Breaking Change (2026-01):** Canonical name `AINCRAD` → `AIN`

</div>

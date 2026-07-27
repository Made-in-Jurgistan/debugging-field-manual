<div align="center">

# <img src="https://api.iconify.design/lucide:bug.svg?color=%23a82828" width="28" height="28" alt="" /> Debugging Field Manual

### Language-Agnostic Strategies · Instrumentation · AI-Augmented Workflows

**30 Sections · Python · Kotlin · C/C++ · Java · TypeScript · Distributed Systems**

[![Version](https://img.shields.io/badge/version-2026.2.0-a82828?style=flat-square)](https://Made-in-Jurgistan.github.io/debugging-field-manual/)
[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-a82828?style=flat-square)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Accessibility](https://img.shields.io/badge/WCAG-2.2%20AA-a82828?style=flat-square)](https://www.w3.org/TR/WCAG22/)
[![Print Ready](https://img.shields.io/badge/print-A4%20ready-a82828?style=flat-square)](https://Made-in-Jurgistan.github.io/debugging-field-manual/)

</div>

---

> **From mindset to postmortem** — 30 sections covering every debugging technique for finding
> and fixing any bug in any system. Includes AI-assisted debugging, MCP tool integration,
> distributed tracing, eBPF observability, and blameless root cause analysis.

---

## <img src="https://api.iconify.design/lucide:book-open.svg?color=%23a82828" width="20" height="20" alt="" /> Table of Contents

| # | Section | Group | Focus |
| --- | --------- | ------- | ------- |
| 00 | About This Guide | Orientation | Audience, structure, how to use |
| 01 | The Debugging Mindset | Orientation | Psychological approach, curiosity, patience |
| 02 | Problem Framing & Triage | Orientation | Reproduction, isolation, severity assessment |
| 03 | Articulation & Rubber Ducking | Core Methods | Forced precision, verbalization techniques |
| 04 | The Hypothesis Loop | Core Methods | Scientific method applied to debugging |
| 05 | Reading Errors Effectively | Core Methods | Stack traces, error chains, signal vs noise |
| 06 | Binary Search Debugging | Core Methods | `git bisect`, comment-out, delta isolation |
| 07 | Logging Strategy | Instrumentation | Structured logging, levels, correlation IDs |
| 08 | Breakpoints & Step Debugging | Instrumentation | `lldb`, `gdb`, `pdb`, IntelliJ debugger |
| 09 | Distributed Tracing | Instrumentation | OpenTelemetry, Jaeger, Honeycomb, Grafana |
| 10 | Performance Profiling | Instrumentation | `py-spy`, `memray`, `bpftop`, `perf`, `bpftrace` |
| 11 | Network & API Debugging | Domain-Specific | `tcpdump`, `Wireshark`, `mitmproxy`, `curl` |
| 12 | Database & Query Debugging | Domain-Specific | EXPLAIN ANALYZE, lock detection, N+1 queries |
| 13 | Memory Debugging | Domain-Specific | ASan, Valgrind, `memray`, leak detection |
| 14 | Concurrency & Race Conditions | Domain-Specific | Thread sanitizers, happens-before, deadlocks |
| 15 | Browser & Frontend | Domain-Specific | DevTools, source maps, React Profiler |
| 16 | Error Handling Design | Error Handling | Result types, error propagation, resilience |
| 17 | Static Analysis & Linting | Error Handling | Clang-Tidy, Ruff, ESLint, SonarQube |
| 18 | Monitoring & Alerting | Error Handling | SLO/SLI, alert fatigue, dashboards |
| 19 | AI-Assisted Debugging | AI & Agents | LLM debugging, context engineering, prompting |
| 20 | MCP Tools for Debugging | AI & Agents | Model Context Protocol, tool integration |
| 21 | Debugging AI Agents | AI & Agents | Agent loops, tool call tracing, hallucination |
| 22 | Agentic Debug Workflows | AI & Agents | Multi-agent debugging, autonomous triage |
| 23 | Production Debugging | Production | Hot vs cold, safe instrumentation, rollbacks |
| 24 | Debugging in CI/CD | Production | Flaky tests, environment drift, reproducibility |
| 25 | Root Cause Analysis & Postmortems | Production | Blameless RCA, 5 Whys, fishbone diagrams |
| 26 | The 2026 Toolkit Reference | Reference | Every tool organized by problem domain |
| 27 | Anti-Patterns & Traps | Reference | Common pitfalls, cognitive biases, time sinks |
| 28 | Master Debugging Checklist | Reference | Pre- and post-debug quality protocol |
| 29 | Index & Resources | Reference | Curated library of books, papers, and tools |

---

## <img src="https://api.iconify.design/lucide:key-round.svg?color=%23a82828" width="20" height="20" alt="" /> Key Technologies

| Category | Technologies |
|----------|-------------|
| **Tracing** | OpenTelemetry, Jaeger, Honeycomb, Grafana, eBPF (`bpftrace`, `pwru`, `kyanos`) |
| **Profiling** | `py-spy`, `memray`, `bpftop`, `perf`, `Valgrind`, ASan, `parca`, `pyroscope` |
| **Debuggers** | `gdb`, `lldb`, `pdb`, IntelliJ IDEA, Chrome DevTools |
| **Network** | `tcpdump`, `Wireshark`, `mitmproxy`, `curl`, `nc` |
| **Static Analysis** | Clang-Tidy, Ruff, ESLint, SonarQube, Inspektor Gadget |
| **AI/MCP** | LLM-assisted debugging, Model Context Protocol, agent workflows |
| **Languages** | Python, Kotlin, C/C++, Java, TypeScript, Go |
| **Observability** | Odigos, DeepFlow, structured logging, SLO/SLI design |

---

## <img src="https://api.iconify.design/lucide:sparkles.svg?color=%23a82828" width="20" height="20" alt="" /> Guide Features

- **<img src="https://api.iconify.design/lucide:ruler.svg?color=%23a82828" width="16" height="16" alt="" /> Print-Ready** — A4 duplex margins, page-break controls, print-safe color resets
- **<img src="https://api.iconify.design/lucide:accessibility.svg?color=%23a82828" width="16" height="16" alt="" /> WCAG 2.2 AA** — Keyboard navigation, skip links, `:focus-visible` outlines, reduced-motion support, forced-colors support
- **<img src="https://api.iconify.design/lucide:search.svg?color=%23a82828" width="16" height="16" alt="" /> SEO Optimized** — Open Graph, JSON-LD `TechArticle` structured data, canonical URL
- **<img src="https://api.iconify.design/lucide:palette.svg?color=%23a82828" width="16" height="16" alt="" /> Editorial Design** — Lora (display) · DM Sans (body) · JetBrains Mono (code); warm paper palette with crimson accent (`#a82828`)
- **<img src="https://api.iconify.design/lucide:smartphone.svg?color=%23a82828" width="16" height="16" alt="" /> Responsive** — CSS-only sidebar navigation, mobile hamburger menu, scroll progress indicator
- **<img src="https://api.iconify.design/lucide:zap.svg?color=%23a82828" width="16" height="16" alt="" /> Performance** — `content-visibility: auto`, `@property` typed custom properties, layered CSS architecture
- **<img src="https://api.iconify.design/lucide:rainbow.svg?color=%23a82828" width="16" height="16" alt="" /> Wide Gamut** — `color-gamut: p3` media query with OKLCH accent colors

---

## <img src="https://api.iconify.design/lucide:rocket.svg?color=%23a82828" width="20" height="20" alt="" /> Getting Started

### Read Online

Visit the hosted guide: **[Made-in-Jurgistan.github.io/debugging-field-manual](https://Made-in-Jurgistan.github.io/debugging-field-manual/)**

### Read Locally

```bash
git clone https://github.com/Made-in-Jurgistan/Made-in-Jurgistan.github.io.git
cd Made-in-Jurgistan.github.io/debugging-field-manual
open Debugging_Field_Manual.html
# or serve locally:
python -m http.server 8000
# navigate to http://localhost:8000
```

### Print to PDF

Open the HTML file in Chrome/Edge → `Ctrl+P` → set paper size to A4 → enable background graphics → print to PDF.

---

## <img src="https://api.iconify.design/lucide:brain.svg?color=%23a82828" width="20" height="20" alt="" /> The Debugging Methodology at a Glance

```text
  ┌──────────────┐     ┌──────────────┐     ┌──────────────┐
  │   Reproduce  │ ──▶ │   Isolate    │ ──▶ │  Hypothesize │
  └──────────────┘     └──────────────┘     └──────────────┘
                                                    │
  ┌──────────────┐     ┌──────────────┐            ▼
  │   Verify     │ ◀── │    Fix       │ ◀── ┌──────────────┐
  └──────────────┘     └──────────────┘     │    Test      │
                                            └──────────────┘
                                                    ▲
  ┌──────────────┐     ┌──────────────┐            │
  │  Postmortem  │ ◀── │  Document    │ ◀── ┌──────────────┐
  └──────────────┘     └──────────────┘     │   Iterate    │
                                            └──────────────┘
```

---

## <img src="https://api.iconify.design/lucide:library.svg?color=%23a82828" width="20" height="20" alt="" /> Related Guides

| Guide | Focus |
|-------|-------|
| **Mobile STT Engineering Guide** | On-device speech-to-text: audio capture, VAD, model inference, post-processing |
| **Android Keyboard Design Guide** | Production IME development, API 30–36, Material You 3.0 |
| **Android Keyboard: 3D & Personalization** | 3D rendering, PBR materials, custom themes, game engine bridges |

---

## <img src="https://api.iconify.design/lucide:file-text.svg?color=%23a82828" width="20" height="20" alt="" /> Metadata

| Field | Value |
|-------|-------|
| **Author** | Made in Jurgistan |
| **Version** | 2026.2.0 |
| **Published** | 2026-07-24 |
| **Updated** | 2026-07-24 |
| **License** | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| **Accessibility** | WCAG 2.2 AA |
| **Canonical URL** | `https://Made-in-Jurgistan.github.io/debugging-field-manual/` |
| **Theme Color** | `#a82828` (Crimson) |
| **Fonts** | Lora · DM Sans · JetBrains Mono |

---

## <img src="https://api.iconify.design/lucide:git-pull-request.svg?color=%23a82828" width="20" height="20" alt="" /> Contributing

Report issues or suggest improvements: [github.com/Made-in-Jurgistan/debugging-field-manual-2026/issues](https://github.com/Made-in-Jurgistan/debugging-field-manual-2026/issues)

---

## <img src="https://api.iconify.design/lucide:scale.svg?color=%23a82828" width="20" height="20" alt="" /> License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) — Free to share and adapt with attribution. See [`LICENSE-Debugging.md`](LICENSE-Debugging.md) for details.

---

## <img src="https://api.iconify.design/lucide:quote.svg?color=%237c3aed" width="20" height="20" alt="" /> How to Cite

If you reference this guide in academic work, documentation, or project READMEs, please use one of the formats below. Both are consistent with the output generated by GitHub's "Cite this repository" button and the [`cffconvert`](https://github.com/citation-file-format/cffconvert) tool from the repository's `CITATION.cff` file.

### APA (7th Edition)

```text
Made in Jurgistan. (2026). Debugging Field Manual (Version 2026.2.0) [Computer software]. https://Made-in-Jurgistan.github.io/debugging-field-manual/
```

### BibTeX

```bibtex
@software{Made_in_Jurgistan_Debugging_Field_2026,
  author = {Made in Jurgistan},
  month = {7},
  title = {{Debugging Field Manual}},
  url = {https://Made-in-Jurgistan.github.io/debugging-field-manual/},
  version = {2026.2.0},
  year = {2026}
}
```

> **Note:** A `CITATION.cff` file at the repository root also enables GitHub's built-in "Cite this repository" button (right sidebar on the repo page), which auto-generates APA and BibTeX citations from the same metadata.

---

<div align="center">

**Made in Jurgistan** — Complete Edition · 2026

</div>

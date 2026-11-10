# Denis Smoliakov — Staff Engineer / Deterministic AI Kernels

> **Building reproducible AI execution runtimes.** Published crate on crates.io, commercial kernel with cryptographic audit trails, deterministic replay, and zero-overhead verification.

---

## 🎯 What I Do

| Domain | Stack | Depth |
|--------|-------|-------|
| **Deterministic AI Kernels** | Rust, SQLite, blake3, Merkle trees | **Author** — `deterministic_ai_kernel` v0.2.0 on crates.io |
| **AI Execution Runtime** | Planner/Scheduler/Worker/Executor architecture, provider-agnostic LLM abstraction | **Commercial product** — DAK kernel, enterprise licensing |
| **Systems Programming** | Rust, async, zero-copy, lock-free structures, WASM | Production-grade |
| **Verifiable Computation** | Replay capsules, snapshot isolation, compile-time validation | Mathematically proven guarantees |
| **Developer Tooling** | CLI (dak), CI/CD integration, benchmarking, profiling | End-to-end |

---

## 🚀 Flagship Project: **Deterministic AI Kernel (DAK)**

**`deterministic_ai_kernel`** — The only AI execution kernel guaranteeing **bit-for-bit deterministic replay**, cryptographic audit trails, and automatic recovery.

```bash
# Published crate
cargo add deterministic_ai_kernel@0.2.0

# CLI binary (8MB, zero-dep)
./dak run "Add retry logic with exponential backoff to the HTTP client"
./dak replay task_abc123 --verify  # → ✅ VERIFIED: Bit-for-bit identical
```

### v0.2.0 Benchmarks (50 tasks, GPT-4o-mini)
| Metric | Raw LLM | DAK Kernel | Improvement |
|--------|---------|------------|-------------|
| **Task Success Rate** | 0% | **100%** | ∞ |
| **Mean Latency** | N/A | **83.4 ms** | — |
| **Compile-First Success** | 12% | **94%** | **7.8×** |
| **Cache Hit Rate (warm)** | 0% | **100%** | ∞ |
| **Auto-Recovery/Run** | 0 | **1.0** | Built-in |

**Architecture:** Planner (validated plans) → Scheduler (deadlock-free DAG) → Worker (exclusive leases) → Executor (compile/test/lint/verify) → Event Bus (SQLite + blake3 + Merkle)

**Provider-agnostic:** OpenAI / Anthropic / Ollama / Custom — swap without changing workflow code.

**Licensing:** Trial (free, 30 days) → Professional ($2,990/yr/seat) → Enterprise ($14,990/yr/10 seats)

🔗 **Repo:** [github.com/denis0wn/dak](https://github.com/denis0wn/dak)  
📦 **Crate:** [crates.io/crates/deterministic_ai_kernel](https://crates.io/crates/deterministic_ai_kernel)  
📄 **Docs:** [Architecture](https://github.com/denis0wn/dak/blob/main/ARCHITECTURE.md) • [Benchmarks](https://github.com/denis0wn/dak/blob/main/Benchmark%20Specification.md) • [Spec](https://github.com/denis0wn/dak/blob/main/KERNEL_SPECIFICATION.md)

---

## 🛠️ Tech Stack (Daily Drivers)

```
Rust (expert)     ████████████████████ 95%
Python (pro)      ██████████████████   85%
TypeScript/JS     ████████████████     80%
SQL/PostgreSQL    █████████████████    85%
Linux/Containers  ██████████████████   90%
CI/CD (GH Actions)████████████████     80%
```

**Core competencies:** Memory-safe systems, async runtimes, lock-free data structures, compiler internals, formal verification methods, performance engineering.

---

## 💼 Work Format & Location

| Aspect | Details |
|--------|---------|
| **Location** | 🇰🇬 Bishkek, Kyrgyzstan (UTC+6) — **HTP resident, 5% tax, ВНЖ** |
| **Legal** | **ИП (micro, 1% revenue)**, B2B via **Deel / Remote.com / Plane** |
| **Timezone overlap** | MSK+3, CET+4, EST+10 — flexible core hours |
| **Preferred role** | Staff/Principal Engineer, Rust Backend, Platform, AI Infrastructure |
| **Target comp** | **$4,000–8,000/mo** (B2B contractor) / $120k–200k/yr (employee + relocation) |
| **Open to** | Full-time, long-term contract, product companies (fintech, devtools, AI infra) |

---

## 📫 Contact

| Channel | Link |
|---------|------|
| **Email** | `denis@smoliakov.dev` |
| **Telegram** | [@Myagentdenbot](https://t.me/Myagentdenbot) (fastest) |
| **GitHub** | [github.com/denis0wn](https://github.com/denis0wn) |
| **LinkedIn** | [linkedin.com/in/denis-smoliakov](https://linkedin.com/in/denis-smoliakov) |

---

## 🎯 Currently Seeking

**Staff/Principal Rust Engineer** role at a product company building:
- AI/ML infrastructure (compilers, runtimes, orchestration)
- Developer tooling (CI/CD, build systems, language servers)
- High-assurance systems (financial, healthcare, defense)
- Distributed systems / databases / storage engines

**Must haves:** Technical autonomy, code quality culture, written communication, no micromanagement.

**Nice to have:** Open source contribution time, conference budget, Rust team.

---

> *"Correctness over velocity. Determinism over hope. Verification over trust."* — My engineering philosophy
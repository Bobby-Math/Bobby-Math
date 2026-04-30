# Bobby Mathews

Rust systems engineer. I build distributed systems infrastructure 
and write about the difficult parts.

Correctness is not optional — formal verification, cryptographic guarantees, measured latency

---

### Current Work

- **[synkti](https://synkti.com)** — Constrained document 
  verification engine for patent prosecution. Formal grammar 
  verification in WASM, local LLM inference via WebGPU. 
  Ongoing research at [synkti.com](https://synkti.com).

- **[solana-realtime-indexer](https://github.com/Bobby-Math/solana-realtime-indexer)**  — High-performance 
  Solana data pipeline: RPC connection pool + Geyser gRPC 
  consumer → TimescaleDB → public query API. 
  Measured 24ms slot-to-database write latency on devnet.
  40+ TPS sustained.
  Live dashboard: [solana.bobby-math.dev](https://solana.bobby-math.dev)
  
- **[key-sign](https://github.com/Bobby-Math/key-sign)** — Secure Solana key 
  management and signing tool. AES-256-GCM encrypted private keys with 
  Argon2 key derivation, phantom-type safety for key lifecycle, and 
  zeroization. No password recovery by design.

---

### Published Work

- **[tokio-blocking-bench](https://bobby-math.github.io/tokio-blocking-bench)**
  Link: https://bobby-math.github.io/tokio-blocking-bench/
  — Controlled benchmark isolating Tokio executor starvation 
  under blocking workloads. Key finding: 101x p99 latency 
  increase under starvation. EC2-controlled environment, 
  reproducible results.

- **Technical writing** 
  → [Writing samples](https://bobby-math.dev/blog)
  
### Prior Systems Work

- **[synkti-fleet](https://github.com/Bobby-Math/synkti-fleet-public)** — Spot instance orchestration 
  prototype. EC2 tag-based worker discovery, interruption-aware 
  draining, stateless failover. Worked end-to-end; not pursued 
  for economic reasons.
---

### Interests

Async Rust internals · Solana infrastructure · 
Formal verification · High-throughput data pipelines · 
Systems performance benchmarking

---

[bobby-math.dev](https://bobby-math.dev) · 
[LinkedIn](https://www.linkedin.com/in/bobby-math/) · 
[bobby@bobby-math.dev](mailto:bobby@bobby-math.dev)

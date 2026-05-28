# Bobby Mathews

Rust/wgpu systems engineer. I build GPU-accelerated real-time visualization
for high-frequency sensor data.

Correctness is not optional: formal verification, cryptographic guarantees, measured latency.

---

### Focus

Real-time rendering of high-frequency, multi-channel sensor streams in Rust and wgpu.
Ring-buffer ingestion, GPU compute-shader signal processing, single-draw-call rendering
at 60fps, native and in-browser via WASM/WebGPU. One architecture pattern across domains:
research instrumentation, biosignals, robotics, industrial sensors.

The bottleneck in real-time sensor visualization is architectural, not domain-specific.
CPU renderers iterate samples serially and issue draw calls per channel, hitting a ceiling
independent of domain. The GPU-correct path moves the per-sample work to compute and renders
all channels in one pass, inside the frame budget.


---

### Current Work

- **[solana-realtime-indexer](https://github.com/Bobby-Math/solana-realtime-indexer)** :
  Production real-time data pipeline. Lock-free hot path, Geyser gRPC consumer to
  TimescaleDB, public query API, WAL crash recovery. 40+ TPS sustained, slot-to-db
  latency p50 1281ms / p99 1859ms. The high-throughput streaming and latency-discipline
  work the visualization ingestion layer builds on.
  Live dashboard: [solana.bobby-math.dev](https://solana.bobby-math.dev)

- **[key-sign](https://github.com/Bobby-Math/key-sign)** :
  Secure key management and signing tool. AES-256-GCM encrypted keys with Argon2
  derivation, phantom-type safety for key lifecycle, zeroization. No password recovery
  by design.

- **[synkti](https://synkti.com)** :
  Constrained document verification engine. Formal grammar verification in WASM,
  client-side LLM inference via WebGPU. Ongoing research at [synkti.com](https://synkti.com).

---

### Published Work

- **[tokio-blocking-bench](https://bobby-math.github.io/tokio-blocking-bench/)** :
  Controlled benchmark isolating Tokio executor starvation under blocking workloads.
  Key finding: 101x p99 latency increase under starvation. EC2-controlled, reproducible.

- **Technical writing** : [samples](https://bobby-math.dev/blog)

---

### Prior Systems Work

- **[synkti-fleet](https://github.com/Bobby-Math/synkti-fleet-public)** :
  Spot instance orchestration prototype. EC2 tag-based worker discovery,
  interruption-aware draining, stateless failover. Worked end-to-end; not pursued
  for economic reasons.

---

### Interests

Real-time GPU rendering (wgpu/WGSL) · GPU compute · Async Rust internals ·
High-throughput data pipelines · Formal verification · Systems performance benchmarking

---

[bobby-math.dev](https://bobby-math.dev) ·
[bobby@bobby-math.dev](mailto:bobby@bobby-math.dev) ·
[LinkedIn](https://www.linkedin.com/in/bobby-math/)

## Distributed Systems & Compute Infrastructure

I build protocols that make volatile resources production-ready. My work focuses on intelligent orchestration, fault tolerance, and optimizing the intersection of AI compute and decentralized networks.

**Current Focus:**
*   **[Synkti](https://github.com/bobby-math/synkti)**: Domain-agnostic orchestration for spot instances using Kuhn-Munkres optimal migration and grace-period checkpoint recovery. Achieves 70-80% cost reduction while maintaining production reliability.
*   **[Synapse](https://github.com/bobby-math/synapse)**: High-performance CUDA FFI library with optimized GPU kernels. Rust-safe bindings for matrix operations, memory management, and tensor core acceleration. Used as the compute foundation for ML inference and GPU workloads.
*   **[Axon](https://github.com/bobby-math/axon)**: Lightweight ML inference server optimized for LLM serving. Handles model loading, KV cache management, and inference execution with minimal overhead. Built on Synapse for GPU acceleration.

**Core Thesis:**
Compute scarcity is a coordination problem. Stranded inventory (spot instances, consumer GPUs) offers 4-5x capacity expansion if orchestrated with provably optimal scheduling logic.

**Stack:**
*   **Languages:** Rust (primary), C++/CUDA (accelerator kernels)
*   **Specialization:** Rust FFI, systems orchestration, discrete-event simulation
*   **Systems:** Solana, AWS Spot, DePIN infrastructure
*   **Interests:** Mechanism Design, Control Theory, Distributed Runtime Optimization

[bobby-math.dev](https://bobby-math.dev)

![Crates](https://img.shields.io/badge/crates-900-orange)
![SLoC](https://img.shields.io/badge/SLoC-~36M-blue)
![Tests](https://img.shields.io/badge/tests-passing-brightgreen)
[![Discussions](https://img.shields.io/badge/Discussions-%F0%9F%92%AC-blue?logo=github&style=flat)](https://github.com/cool-japan/cool-japan/discussions)

# COOLJAPAN

**One of the largest pure-Rust sovereignty stacks in history.**

The official COOLJAPAN Pure Rust Ecosystem — 900 crates, ~36M SLoC, zero C/FFI (in default) · Memory-safe by design.
We are rebuilding the entire scientific, media, AI, semantic web, formal verification, and systems stack in pure Rust — so AI agents and critical software can run anywhere with full sovereignty.
Playground: https://play.cooljapan.dev/

---

### 📊 Ecosystem at a Glance (August 2026)
- **Total crates**: 900+ (and growing daily)
- **Total Rust SLoC**: ~36 million (Mostly the same as Linux Kernel)
- **Total Rust Files**: 100,000+
- **Passing tests**: 400,000+
- **Projects**: 75+ production-grade libraries
- **All projects**: 100% `fail0` + `Clippy0` enforced

---

### 🚀 Core Projects

| Category                          | Project            | Description                                                                 | Link |
|-----------------------------------|--------------------|-----------------------------------------------------------------------------|------|
| **Scientific Computing**          | SciRS2             | Complete NumPy/SciPy/scikit-learn replacement (~3M SLoC)                    | [→](https://github.com/cool-japan/scirs) |
| **Scientific Computing**          | OxiPhysics         | Unified physics engine - Bullet/OpenFOAM/LAMMPS/CalculiX replacement        | [→](https://github.com/cool-japan/oxiphysics) |
| **LLM**                           | OxiBonsai          | Pure Rust 1-Bit (Sub-2-Bit) LLM Inference Engine + IMAGEN for PrismML Bonsai Models  | [→](https://github.com/cool-japan/oxibonsai) |
| **LLM**                           | OxiLLaMa           | Pure Rust LLM inference engine — the sovereign alternative to llama.cpp     | [→](https://github.com/cool-japan/oxillama) |
| **GPU (CUDA)**                    | OxiCUDA            | NVIDIA CUDA Toolkit software stack with type-safe, memory-safe Rust code    | [→](https://github.com/cool-japan/oxicuda) |
| **Media & Computer Vision**       | OxiMedia           | FFmpeg + OpenCV replacement (108 crates)  (~3M SLoC)                      | [→](https://github.com/cool-japan/oximedia) |
| **Geospatial**                    | OxiGeo            | Pure Rust geospatial data processing engine — cloud-native, full CRS & format support               | [→](https://github.com/cool-japan/oxigeo) |
| **Deep Learning**                 | ToRSh              | PyTorch-compatible framework with native sharding                           | [→](https://github.com/cool-japan/torsh) |
| **Semantic Web & AI Reasoning**   | OxiRS          | Rust-native platform for Semantic Web, SPARQL 1.2, GraphQL, Digital Twin (Apache Jena replacement) | [→](https://github.com/cool-japan/oxirs) |
| **Scientific Computing**          | QuantRS2           | Full Quantum Computing Framework (QuantRS2)                                 | [→](https://github.com/cool-japan/quantrs) |
| **Digital Humans**                | OxiHuman           | Privacy-first parametric human body generator (WASM/WebGPU)                 | [→](https://github.com/cool-japan/oxihuman) |
| **Digital Humans**                | OxiGAF             | Gaussian avatar reconstruction from monocular video                         | [→](https://github.com/cool-japan/oxigaf) |
| **Formal Verification**           | OxiLean            | Memory-safe Interactive Theorem Prover (Lean 4 inspired)                    | [→](https://github.com/cool-japan/oxilean) |
| **Formal Verification**           | OxiZ               | High-performance SMT solver (Z3 replacement)                                | [→](https://github.com/cool-japan/oxiz) |
| **Pure Rust Demo (EML)**           | Phop               | Differentiable symbolic-discovery engine written entirely in pure Rust     | [→](https://github.com/cool-japan/phop) |
| **Legal Technology**              | Legalis-RS (legalis)| Legal statute parser, analyzer & simulator (Legal DX)                       | [→](https://github.com/cool-japan/legalis) |
| **Government Technology (GovTech)** | OxigenAI         | OxigenAI rebuilds the (Japan) Digital Agency's government AI legal system "GenAI", powered by Legalis-RS and OxiZ   | [→](https://github.com/cool-japan/oxigenai) |
| **XML**   | OxiXML            | Pure Rust libraries of XSLT 3.0 / XQuery / XSD 1.1 / RELAX NG / Schematron / XMLDSig / XSL-FO / RDF 1.2 / Turtle / RDF-XML / JSON-LD / RDFa / SVG / canonicalization / SPARQL     | [→](https://github.com/cool-japan/oxixml) |
| **Ephemeris**   | OxiEphemeris            | A pure-Rust, clean-room astronomical ephemeris engine (esp. for Astrology)     | [→](https://github.com/cool-japan/oxiephemeris) |
| **Real-time Signal Processing**   | Kizzasi            | Rust-native AGSP for continuous audio, sensor, robotics & video streams     | [→](https://github.com/cool-japan/kizzasi) |
| ...                               | 60+ more projects  | Full ecosystem overview at [cooljapan.tech](https://cooljapan.tech)                                   | — |

**Full project list & latest releases** → [Ecosystem Overview](https://cooljapan.tech)

---

### Monthly COOLJAPAN Article (Third Party) — Call for Articles

Independent write-ups about the COOLJAPAN Pure Rust ecosystem, updated monthly.

Curated by KitaSan — the first individual sponsor of the Apache Software Foundation and the founder of the Apache Newsletter (2003).

- **2026-05** — [1-Bit LLMs in Pure Rust — A field report from OxiBonsai v0.1.3](https://nazquadri.com/blog/everyday-thoughts/oxibonsai-1-bit-pure-rust/) · Naz Quadri
  A hands-on field report: measured decode and prefill throughput across the
  CPU AVX-2 and CUDA backends on real hardware, read through the SIMD kernels
  and error model, and documented three defects. Assesses the source as
  senior-level human Rust, and notes that release count rather than commit
  count is the meaningful activity signal for this codebase.

- **2026-08** — [Local Inference Engine: OxiBonsai](https://discuss.4d.com/t/local-inference-engine-oxibonsai/39077) · 4D Developer Community
  Introduces OxiBonsai as a pure Rust inference engine for PrismML's sub-2-bit
  Bonsai models, noting its OpenAI-compatible server API as a drop-in
  replacement for existing workflows, and its zero C/FFI construction on the
  COOLJAPAN ecosystem.

📚 **[Full archive → cooljapan.tech/articles](https://cooljapan.tech/articles)**

Written about COOLJAPAN? Open an issue at
[cool-japan/cool-japan/issues](https://github.com/cool-japan/cool-japan/issues)
with the link, or email contact@cooljapan.tech — we'll feature it here.

---

### 📚 Resources

- **Tech Blog** (official): [blog.cooljapan.tech](https://blog.cooljapan.tech)
- **Medium** (release announcements): [kitasanio.medium.com](https://kitasanio.medium.com)
- **LinkedIn**: [KitaSan](https://www.linkedin.com/in/tetsuya) -- LinkedIn Member since Feb. 29th, 2004
- **Main Website**: [cooljapan.tech](https://cooljapan.tech)

---

### 🛠 Get Involved

- Star the repos you like
- [Try the WASM demos](https://play.cooljapan.dev/)
- Contribute (we welcome issues)
- Follow the blog for daily release updates

**The Rust sovereignty stack is here.**  
No more C dependencies (in default). No more Python for science. No more cloud lock-in.

Built with ❤️ by COOLJAPAN OÜ / Estonia (KitaSan, a Rustacean in a rusty, poor village in Southeast Asia)

---

Made with pure Rust • All public • Always `fail0 + Clippy0`

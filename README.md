# Hi, I'm TechPrototyper 👋

## Mission: production-quality AI on consumer hardware

The best models shouldn't require a datacenter. I work on making **local AI
measurably excellent** — maximum compression and speed with *no quality left
on the table* — on machines enthusiasts and small teams actually own:
consumer GPUs like the RTX 5090, and entry-level AI systems like the
GB10-class DGX Spark.

The bottleneck on this hardware is never compute — it's memory. So that's
where I work:

- **KV-cache compression & quantization** on consumer Blackwell
  (sm_120 / sm_121): NVFP4 today — rotation-based paths measured (and
  respectfully shelved), sub-4-bit next — with a soft spot for the hard
  cases: hybrid attention layouts, heterogeneous head dimensions,
  calibrated scales.
- **Upstream first.** I contribute to and validate for
  [vLLM](https://github.com/vllm-project/vllm) and
  [FlashInfer](https://github.com/flashinfer-ai/flashinfer).
  Evidence over opinion: measured, reproducible, disclosed.
- 📓 **Lab notebook:** [local-ai-lab](https://github.com/TechPrototyper/local-ai-lab)
  — what I measure, how it turns out, and the recipes it leads to.
- **Mixed-precision weights, speculative decoding, smart offloading** —
  every technology that turns a 32 GB ceiling from a wall into a
  well-managed budget.

## Merged upstream

Receipts, not claims — each of these was reviewed and merged by the project's own maintainers:

- **agentgateway** [#3393](https://github.com/agentgateway/agentgateway/pull/3393) — configurable SSE keep-alive for long-lived MCP streams; shipped in `v1.6.0-alpha.1`
- **FlashInfer** [#3684](https://github.com/flashinfer-ai/flashinfer/pull/3684) — asymmetric VO-split NVFP4 paged prefill (qk=512 / vo=256) for Gemma-4 on SM120/121, co-authored with [@jethac](https://github.com/jethac)
- **prismaquant** [#80](https://github.com/RobTand/prismaquant/pull/80) — hybrid linear-attention masking in layer streaming for Qwen3.5/3.6 on transformers ≥ 5.15
- **jethac/vllm** [#1](https://github.com/jethac/vllm/pull/1) — NVFP4 FA2 per-page KV layout: fixes hybrid-model corruption while keeping full tensor sharing, in the fork behind [vllm-project/vllm#46329](https://github.com/vllm-project/vllm/pull/46329)
- **mcp-server-devonthink** [#31](https://github.com/dvcrn/mcp-server-devonthink/pull/31) — `createRecord` now returns the reference URL
- **tpk** [#2](https://github.com/apuder/tpk/pull/2) — Space Invaders for the TRS-80 Model I and Model III (see *Off the clock*)

In review at vllm-project/vllm: [#53977](https://github.com/vllm-project/vllm/pull/53977) · [#53978](https://github.com/vllm-project/vllm/pull/53978) · [#53979](https://github.com/vllm-project/vllm/pull/53979) — speculative-decoding and NVFP4-KV fixes for consumer Blackwell.

## Habitat

Solution & integration architect by trade — I build systems that stay
elegant under real-world constraints.
Linux · Kubernetes (Talos, Flux/GitOps) · Azure · Python.
Homelab: a K8s cluster with an RTX 5090, an ASUS Ascent GX10 (GB10),
and more retro hardware than strictly necessary.

## Off the clock

Retro computing enthusiast — the machines that taught us that constraints
breed elegance. Which, come to think of it, is the mission statement again.

A European with an honest affection for America.

---

*My contributions are often AI-assisted and always human-directed and
human-validated — each one carries a disclosure line, per the projects'
policies.*

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
  (sm_120 / sm_121): NVFP4 today, rotation-based and sub-4-bit paths next —
  with a soft spot for the hard cases: hybrid attention layouts,
  heterogeneous head dimensions, calibrated scales.
- **Upstream first.** I contribute to and validate for
  [vLLM](https://github.com/vllm-project/vllm) and
  [FlashInfer](https://github.com/flashinfer-ai/flashinfer).
  Evidence over opinion: measured, reproducible, disclosed.
- **Mixed-precision weights, speculative decoding, smart offloading** —
  every technology that turns a 32 GB ceiling from a wall into a
  well-managed budget.

## Habitat

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

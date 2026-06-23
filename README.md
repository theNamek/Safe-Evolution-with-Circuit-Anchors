# Safe Evolution with Circuit Anchors

📄 **[Paper PDF](./Safe-Evolution-with-Circuit-Anchors.pdf)**

**Status:** Preprint. Under review.

## Overview

Current self-evolution algorithms for LLMs optimize purely for capability, causing models to *misevolve* — becoming powerful yet losing safety alignment. Inspired by how conserved Hox genes anchor biological body plans during evolution, we propose **Circuit-Anchored Evolution (CAE)**: identify a minimal safety circuit (<2% of features) via mechanistic interpretability, then anchor it during evolution while letting everything else adapt freely.

<p align="center">
  <img src="./Overview.jpg" width="600">
</p>

## Key Results

- 📉 **Unconstrained evolution is dangerous:** all models degrade from 96–99% to 70–75% safety score within 500 steps
- 🔒 **CAE preserves safety above 95%** throughout evolution, while unconstrained evolution drops to ~70%
- 🚀 **No capability trade-off:** CAE matches the capability gains of unconstrained evolution, unlike reward-model baselines which sacrifice capability for safety
- ⚡ **Lower overhead than reward models:** only requires activation extraction through frozen transcoders, no additional forward pass through a safety reward model

## Citation

If you find this work useful, please cite:

```bibtex
@misc{liu2026safeevolution,
  title={Safe Evolution with Circuit Anchors},
  author={Yan Liu, Jie Fu, Tsung-Yi Ho},
  year={2026},
  howpublished={\url{https://github.com/theNamek/Safe-Evolution-with-Circuit-Anchors}},
  note={Preprint}
}

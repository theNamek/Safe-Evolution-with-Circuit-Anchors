# Safe Evolution with Circuit Anchors

📄 **[Paper PDF](./Safe-Evolution-with-Circuit-Anchors.pdf)**

**Status:** Preprint. Under review.

## Abstract

In biological evolution, unconstrained mutation can lead to catastrophic outcomes: organisms may evolve enhanced capabilities while losing essential functions for survival. Nature's solution is *developmental constraints*, where core regulatory genes remain anchored while peripheral genes adapt freely. We observe that current self-evolution algorithms for large language models lack analogous constraints. They optimize purely for capability, implicitly assuming safety will be preserved. Our experiments reveal this assumption to be dangerously wrong: models can *misevolve* into powerful yet dangerous entities. Inspired by how Hox genes anchor body structure across 500 million years of evolution, we propose **Circuit-Anchored Evolution (CAE)**. Using mechanistic interpretability, we identify a tiny *safety circuit*, comprising less than 2% of model features, that causally mediates safety behaviors. We anchor this circuit during evolution, constraining it within a small displacement bound while allowing the remaining features to evolve freely. This mirrors the biological principle of *evolvability with constraint*: preserving what is essential while adapting what is peripheral. Experiments across 3 model families and two evolution algorithms demonstrate that CAE achieves superior safety preservation with minimal capability loss, substantially outperforming explicit reward-based constraints in both effectiveness and efficiency. Just as developmental constraints prevent biological evolution from producing nonviable organisms, circuit anchoring prevents model evolution from producing capable but dangerous systems.

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

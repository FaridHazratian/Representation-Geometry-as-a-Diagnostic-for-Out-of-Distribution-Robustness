# Representation-Geometry-as-a-Diagnostic-for-Out-of-Distribution-Robustness

## Summary

In this article, we conducted a research to investigate how geometric and topological properties of learned representation spaces relate to robustness under distribution shift. Rather than relying solely on predictive performance, we study whether intrinsic structural characteristics of deep embeddings can serve as reliable diagnostics for out-of-distribution (OOD) generalization.

Specifically, we analyze representations learned by modern neural architectures across multiple training checkpoints and corruption benchmarks, and quantify their geometry using graph-based and spectral invariants. Our central hypothesis is that models exhibiting simpler global spectral structure and smoother local geometry in representation space tend to generalize better under distribution shifts.

## Key Contributions

- Construction of **class-conditional k-NN graphs** over deep embeddings extracted from trained models.
- Introduction and evaluation of two complementary **geometry-based metrics**:
  - **Global spectral complexity** via log-determinant–based torsion proxies of the normalized graph Laplacian.
  - **Local smoothness** via discrete Ollivier–Ricci curvature.
- Systematic analysis of **checkpoint-level correlations** between geometric metrics and OOD accuracy.
- Empirical validation across multiple datasets and corruption severities.
- **Joint geometry analysis** combining global and local invariants to better explain robustness behavior.

---

## Datasets

The experiments are conducted on standard in-distribution and out-of-distribution benchmarks, including:

- CIFAR-10  
- CIFAR-10.1 / CIFAR-10.2  
- CIFAR-10-C  
- Tiny-ImageNet-C  

Pre-trained models and checkpoints are evaluated consistently across all corruption types and severity levels.


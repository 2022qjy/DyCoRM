<div align="center">

# DyCoRM: Dynamic Criterion-Aware Reward Modeling for Text-to-Image Generation

**NeurIPS 2026 Poster**

Jiaying Qian<sup>*</sup>, Ziheng Jia<sup>*</sup>, Qian Zhang, Zicheng Zhang,<br>
Jiayi Guo, Junqi Zhang, Guangtao Zhai, Xiongkuo Min<sup>&dagger;</sup>

Shanghai Jiao Tong University

<sup>*</sup>Equal contribution. <sup>&dagger;</sup>Corresponding author.

[Paper](https://openreview.net/forum?id=zzottG3vbp) | DyCoDataset-20K: TBA | DyCoBench-1K: TBA | Model Weights: TBA

</div>

## Release Status

This repository provides the datasets and final model weights accompanying our paper. The planned resources are DyCoDataset-20K, DyCoBench-1K, and the final DyCoRM checkpoint. Download links and final package details will be added when the corresponding resources are available.

| Resource | Planned contents | Status | Download |
| --- | --- | --- | --- |
| **DyCoDataset-20K** | Generated images, prompts, image-pair metadata, human-written criteria, criterion-level and overall preference annotations, and training split manifests | Pending release | TBA |
| **DyCoBench-1K** | Held-out benchmark images, evaluation pairs, criteria, preference labels, and evaluation manifests for single-criterion, multi-criteria, and overall evaluation | Pending release | TBA |
| **DyCoRM final weights** | Stage-2 criterion-conditioned pairwise comparison checkpoint, including the comparison head and model configuration | Pending release | TBA |

- [ ] Release DyCoDataset-20K.
- [ ] Release DyCoBench-1K.
- [ ] Release the final DyCoRM weights.

## Introduction

DyCoRM models text-to-image preferences under task-relevant, fine-grained criteria. It separates reward modeling into two stages: grounding criteria from the prompt and candidate image pair, then comparing the images under a supplied criterion or criterion set.

This release includes:

- **DyCoDataset-20K**, a dataset with dynamic criteria and human preference annotations.
- **DyCoBench-1K**, a held-out benchmark for criterion-aware image comparison.
- **Final DyCoRM model weights**, for criterion-conditioned pairwise comparison.

## Dataset

### DyCoDataset-20K

Each annotated comparison contains a text prompt, two candidate images, a set of human-written criteria, and the associated criterion-level and overall preference labels. Preference labels distinguish image A, image B, and a tie.

The release will document the annotation fields, label encoding, image identifiers, image-generation sources, and split membership. Final exported sample counts and file sizes will be listed with the downloadable package.

**Download:** TBA.

### DyCoBench-1K

DyCoBench-1K evaluates single-criterion, multi-criteria, and overall preference prediction. The reported split is image-disjoint from both training stages; textual prompts and source-generator families may overlap across splits.

The benchmark release will provide the evaluation manifests, ground-truth labels, and metric definitions for comparison under supplied criteria.

**Download:** TBA.


## Model Weights

DyCoRM uses InternVL-3-8B-Instruct, with Qwen2.5-7B as its language backbone. We plan to release the final criterion-conditioned pairwise comparison checkpoint:

| Checkpoint | Input | Output | Download |
| --- | --- | --- | --- |
| **Final DyCoRM: criterion-conditioned comparison** | Text prompt, two candidate images, and a criterion condition | Pairwise preference prediction | TBA |

The final DyCoRM model compares an image pair rather than assigning a context-independent absolute score to a single image. Checkpoint format, base-model dependencies, and loading instructions will be provided with the released weights.

## Citation

If you use DyCoRM, DyCoDataset-20K, or DyCoBench-1K, please cite our paper. The entry below uses the accepted conference information; final proceedings metadata can be added when available.

```bibtex
@inproceedings{qian2026dycorm,
  title={DyCoRM: Dynamic Criterion-Aware Reward Modeling for Text-to-Image Generation},
  author={Qian, Jiaying and Jia, Ziheng and Zhang, Qian and Zhang, Zicheng and Guo, Jiayi and Zhang, Junqi and Zhai, Guangtao and Min, Xiongkuo},
  booktitle={Advances in Neural Information Processing Systems},
  year={2026},
  url={https://openreview.net/forum?id=zzottG3vbp}
}
```

## Contact

For questions about the project, please contact Jiaying Qian at [2022qjy@sjtu.edu.cn](mailto:2022qjy@sjtu.edu.cn).

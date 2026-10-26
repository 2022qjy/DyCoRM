<div align="center">

  <div>
    <a href="https://openreview.net/forum?id=zzottG3vbp"><img src="https://img.shields.io/badge/Paper-OpenReview-blue" alt="Paper on OpenReview" /></a>
    <img src="https://img.shields.io/badge/NeurIPS-2026%20Poster-orange" alt="NeurIPS 2026 Poster" />
    <a href="#training-dataset"><img src="https://img.shields.io/badge/Dataset-Coming%20Soon-lightgrey" alt="Datasets coming soon" /></a>
    <a href="#model-weights"><img src="https://img.shields.io/badge/Model%20Weights-Coming%20Soon-lightgrey" alt="Final model weights coming soon" /></a>
  </div>

  <h1>DyCoRM: Dynamic Criterion-Aware Reward Modeling for Text-to-Image Generation</h1>

  <p><em>[NeurIPS 2026 Poster] Official datasets and final model weights for DyCoRM</em></p>

  <div>
    <a href="https://github.com/2022qjy">Jiaying Qian</a><sup>1*</sup>,
    Ziheng Jia<sup>1*</sup>,
    Qian Zhang<sup>1</sup>,
  </div>

  <div>
    <a href="https://zzc-1998.github.io/">Zicheng Zhang</a><sup>2</sup>,
    Jiayi Guo<sup>1</sup>,
    Junqi Zhang<sup>1</sup>,
  </div>

  <div>
    <a href="https://ee.sjtu.edu.cn/en/FacultyDetail.aspx?id=24&amp;infoid=153&amp;flag=153">Guangtao Zhai</a><sup>1</sup>,
    <a href="https://scholar.google.com/citations?user=91sjuWIAAAAJ&amp;hl=zh-CN&amp;oi=ao">Xiongkuo Min</a><sup>1#</sup>
  </div>

  <br />

  <div><sup>1</sup>Shanghai Jiao Tong University. <sup>2</sup>Shanghai Artificial Intelligence Laboratory</div>
  <div><sup>*</sup>Equal contribution. <sup>#</sup>Corresponding author.</div>

  <!-- Add the actual GitHub stars and arXiv badges when their URLs are confirmed. -->

  <!-- Uncomment after adding the dataset overview image.
  <div style="width: 100%; text-align: center; margin: auto;">
    <img style="width: 100%;" src="assets/dataset_overview.png" alt="DyCoDataset-20K overview" />
  </div>
  -->

  <!-- Uncomment after adding the framework image.
  <div style="width: 100%; text-align: center; margin: auto;">
    <img style="width: 100%;" src="assets/framework.png" alt="DyCoRM framework" />
  </div>
  -->

</div>

<div align="left">

## TODO

- [ ] Release DyCoDataset-20K.
- [ ] Release DyCoBench-1K.
- [ ] Release the final DyCoRM weights.

All three resources are pending release. Download links will be added below when available.

## Introduction

DyCoRM models text-to-image preferences under task-relevant, fine-grained criteria. It separates reward modeling into two stages: grounding criteria from the prompt and candidate image pair, then comparing the images under a supplied criterion or criterion set.

## Training Dataset

- **DyCoDataset-20K:** TBA (pending release).
- **Human-rated annotations and split manifests:** TBA (pending release).

Each annotated comparison contains a text prompt, two candidate images, a set of human-written criteria, and the associated criterion-level and overall preference labels. Preference labels distinguish image A, image B, and a tie.

The release will include images, prompts, image-pair metadata, criteria, preference annotations, and training split manifests. Annotation fields, label encoding, final sample counts, and package sizes will be documented with the download.

## Benchmark

- **DyCoBench-1K:** TBA (pending release).

DyCoBench-1K evaluates single-criterion, multi-criteria, and overall preference prediction. The reported split is image-disjoint from both training stages; textual prompts and source-generator families may overlap across splits.

The benchmark release will provide the evaluation manifests, ground-truth labels, and metric definitions for comparison under supplied criteria.

## Model Weights

- **Final DyCoRM model weights:** TBA (pending release).

DyCoRM uses InternVL-3-8B-Instruct, with Qwen2.5-7B as its language backbone. The released checkpoint will contain the final criterion-conditioned pairwise comparison model, including its comparison head and model configuration.

The model takes a text prompt, two candidate images, and a criterion condition to predict their relative preference. Checkpoint format, base-model dependencies, and loading instructions will accompany the weights.

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

</div>

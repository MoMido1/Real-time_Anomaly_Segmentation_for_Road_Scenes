# Real-Time Anomaly Segmentation for Road Scenes

This repository is a legacy ERFNet-based research/course-project snapshot for semantic segmentation and out-of-distribution anomaly detection in road scenes. It includes training and evaluation scripts, experiment logs, result summaries, and model checkpoints.

> **Status:** Research code with legacy dependencies. The original instructions target Python 3.6 and PyTorch/CUDA 8.0; current compatibility has not been established. Numerical results in the repository are historical records, not independently reproduced benchmarks.

## What is included

- `ERF_Net/train/` — ERFNet training and data-preparation utilities.
- `ERF_Net/eval/` — anomaly evaluation, IoU, visualization, and timing scripts.
- `ERF_Net/trained_models/` — ERFNet pretrained model files.
- `ERF_Net/save/` — experiment configurations, logs, checkpoints, and a training archive.
- `eval/results.txt` and `ERF_Net/eval/results.txt` — stored metric summaries from prior experiments.
- `Proj_Tasks.pdf` and `Results/BaseLineResults.docx` — project/task and baseline-result documents.

## Related repository

The sibling repository [`real-time-anomaly-segmentation-for-road-scenes`](https://github.com/MoMido1/real-time-anomaly-segmentation-for-road-scenes) is a broader, private research workspace containing additional model families and experiments, including BiSeNet, ENet, ERFNet, and temperature-scaled ERFNet. The public repository here is the smaller ERFNet-focused snapshot. Some ERFNet files, checkpoints, and result records are shared between the two repositories; they should not be treated as two independent projects or independent evaluations.

## Datasets and evaluation

The original workflow refers to:

- [Cityscapes](https://www.cityscapes-dataset.com/) for semantic segmentation.
- Road Anomaly, Road Obstacle, and Fishyscapes for anomaly evaluation.

Download datasets from their official sources and review each dataset's current terms before use. Do not add dataset images or labels to this repository unless redistribution is expressly permitted. Cityscapes' terms prohibit redistributing its dataset and restrict use to non-commercial purposes; model derivatives may be shared only under the conditions specified in its terms, including that they do not allow recovery of the dataset.

## Environment and usage

The original project documented Python 3.6 and PyTorch with CUDA 8.0. These versions are obsolete. Use an isolated environment and expect compatibility work before running the original scripts.

The repository's original command examples and dataset paths may be machine-specific. Review the README files under `ERF_Net/train/` and `ERF_Net/eval/`, then verify the exact script arguments and checkpoint format in this checkout before running an experiment.

For any result you report, record the dataset and split, checkpoint, evaluation protocol, software versions, input resolution, hardware, and metric definitions. The checked-in result files do not by themselves establish a reproducible experiment.

## Checkpoints, results, and licensing

The upstream [ERFNet project](https://github.com/eromera/erfnet) states that its work is licensed under **CC BY-NC 4.0** (attribution required; non-commercial use only). This repository does not currently include a root-level license that establishes the provenance and terms of every local change, experiment checkpoint, archive, or document.

- The upstream ERFNet pretrained weights should be used in accordance with the upstream license and attribution requirements.
- The provenance and redistribution permissions for each locally trained checkpoint and the training ZIP have not been independently verified. Do not assume that every artifact inherits the upstream license automatically.
- Textual metric summaries can be useful research records, but cite the datasets and methods, verify the evaluation protocol, and do not present them as independently reproduced results.
- Before redistributing checkpoints, confirm their origin and that the relevant dataset and code terms permit sharing. If this cannot be confirmed, remove the unverified artifacts from the public repository.

This README is documentation, not a new license grant for third-party code, datasets, checkpoints, or documents.

# CSI-VAE

Official implementation of the paper "Structured Learning of Compositional Sequential Interventions" (NeurIPS 2024).

## Overview

This repository contains the code for training and evaluating the CSI-VAE model, which [brief 1-2 sentence description of what the model does].

## Installation

### Prerequisites
- [Anaconda](https://www.anaconda.com/products/individual#download-section) or Miniconda
- Python 3.8+
- Git

### Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/jialin-yu/CSI-VAE.git
cd CSI-VAE
```

2. Create and activate the conda environment:
```bash
conda env create -f environment.yml -n csi-vae
conda activate csi-vae
```

## Experiments

### Synthetic Data Experiments

1. Generate synthetic data:
   - Run `synthetic/simulator-clean.ipynb`
   - The simulator creates the necessary datasets for all synthetic experiments

2. Train and evaluate models:
   - Execute notebooks in the `synthetic/` directory for different model variants
   - For conformal prediction experiments, use `synthetic/conformal-prediction.ipynb`

**Note**: Ensure consistent random seeds between the simulator and training notebooks for reproducibility.

### Spotify Experiments

1. Data Preparation:
   - Run `preprocess.ipynb` to process the raw data (download link provided in notebook)
   - Alternatively, use `load_data.ipynb` to load pre-processed datasets
   - Generate experimental data using `simulator.ipynb`

2. Training and Evaluation:
   - Navigate to `spotify/` directory
   - Follow individual notebook instructions for specific experiments

### Visualization

Use `visualisation.ipynb` to reproduce figures and visualize experimental results.

## Citation

If you find this code useful for your research, please cite our paper:

```bibtex
@article{yu2024structured,
  title={Structured Learning of Compositional Sequential Interventions},
  author={Yu, Jialin and Koukorinis, Andreas and Colombo, Nicol{\`o} and Zhu, Yuchen and Silva, Ricardo},
  journal={arXiv preprint arXiv:2406.05745},
  year={2024}
}
```

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or issues, please open a GitHub issue or contact one of the authors (jialin.yu@ucl.ac.uk).
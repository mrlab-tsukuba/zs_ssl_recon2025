# Compressed Sensing Reconstruction with Zero-Shot Self-Supervised Learning (ZS-SSL) for High-Resolution MRI of Human Embryos

This repository contains source code used in the study:

> **Compressed Sensing Reconstruction with Zero-Shot Self-Supervised Learning for High-Resolution MRI of Human Embryos**  
> Kazuma Iwazaki, Naoto Fujita, Shigehito Yamada, Kazuyuki Makihara, Yasuhiko Terada  
> _Submitted to Tomography, 2025_

## 📌 Overview

This project implements **zero-shot self-supervised learning (ZS-SSL)** reconstruction for undersampled k-space MRI data, optimized for **high-resolution magnetic resonance microscopy (MRM)** of **human embryos**. The framework allows robust reconstruction from a single undersampled scan without pretraining, enabling significant scan time reduction while preserving spatial resolution.

## 🚀 Quick Start

This project uses **Docker** to ensure a fully reproducible environment across different systems. All dependencies (Python, PyTorch, CUDA, etc.) are preconfigured within a container, avoiding version conflicts and complex local setup.

### 1. Clone the Repository and Launch the Container

Make sure you have [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/) installed.

Then, run the following commands:

```bash
git clone https://github.com/mrlab-tsukuba/zs_ssl_recon2025.git
cd zs_ssl_recon2025
docker compose up -d
```

- This will **build a Docker image** and **start a container** based on the provided `docker-compose.yml` file.
- The container includes all required libraries, Jupyter Lab, and GPU support (if available).

### 2. Access Jupyter Lab

Once the container is running:

- Open your browser and go to: [http://localhost:8888](http://localhost:8888)
- You should see the **Jupyter Lab interface**, served from inside the container.
- Navigate to `sample.ipynb` and follow the cells to run a demo of ZS-SSL reconstruction.

> 📌 If you are running Docker on a remote server, replace `localhost` with the server IP address.


## 🧪 Dataset

- Simulation data: Numerical phantoms with circular/square targets at varying SNRs

> **Note**: Actual data is not included in this repository due to ethical and institutional restrictions.


## 📃 License

This repository is licensed under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).


## 🧑‍🔬 Acknowledgements

This project was supported by JSPS KAKENHI Grant JP21H01333.  
The human embryo data was provided by the Kyoto Collection under ethical approval from Kyoto University.


## 📬 Contact

For questions or collaborations, please contact:

**Yasuhiko Terada**  
[terada.yasuhiko.fu@u.tsukuba.ac.jp](mailto:terada.yasuhiko.fu@u.tsukuba.ac.jp)


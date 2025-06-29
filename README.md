````markdown
# 🔓 Jailbreaking Deep Models: Adversarial Pixel-wise and Patch Attacks on ImageNet Classifiers

> **Authors:** Riya Garg, Kevin Mai, Pranav Bhatt  
> **Affiliation:** NYU Tandon School of Engineering  
> **Course Project – Deep Learning, Spring 2025**  
> **Instructor:** Prof. Chinmay Hegde

---

## 📘 Overview

This project explores the adversarial robustness of deep neural networks using **norm-bounded (ℓ∞) and spatially-constrained attacks** on a ResNet-34 classifier trained on ImageNet. We implement and evaluate:

- **FGSM** (Fast Gradient Sign Method)
- **PGD** (Projected Gradient Descent with 5 iterations)
- **Patch-based PGD** (32×32 local perturbation)

Attacks are evaluated on a 100-class, 500-image ImageNet subset and tested for **transferability** on DenseNet-121.

---

## 🧪 Attack Summary

| **Attack**      | **Top-1 Accuracy (ResNet-34)** | **Top-5 Accuracy** | **Success Rate** |
|-----------------|-------------------------------|---------------------|------------------|
| Clean           | 73.5%                         | 91.2%              | —                |
| FGSM (ε = 0.02) | 26.9%                         | 49.8%              | 73.1%            |
| PGD-5           | 1.6%                          | 11.4%              | 98.4%            |
| Patch (ε = 0.3) | 22.7%                         | 46.4%              | 77.3%            |

See `report.pdf` for detailed analysis, visualizations, transfer performance on DenseNet-121, and runtime benchmarks.

---

## 📁 Files Included

| File                          | Description                                  |
|------------------------------|----------------------------------------------|
| `Jailbreaking_ImageNet.ipynb` | End-to-end adversarial attack notebook       |
| `report.pdf`                 | Final project report with full results        |

---

## 🛠️ Setup Instructions

> Requires: Python ≥ 3.8, PyTorch ≥ 2.2, torchvision, tqdm, matplotlib

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/imagenet-adversarial-attacks.git
   cd imagenet-adversarial-attacks
````

2. Install required packages:

   ```bash
   pip install torch torchvision tqdm matplotlib tabulate scikit-learn
   ```

3. Launch the notebook:

   ```bash
   jupyter notebook Jailbreaking_ImageNet.ipynb
   ```

---

## 📜 License

This project is released under the MIT License. See the `LICENSE` file for details.

---

## 🙏 Acknowledgments

We thank **Prof. Chinmay Hegde** and the **NYU HPC team** for their guidance and computational resources.

```

Let me know if you want:
- A `requirements.txt` auto-generated
- This converted into a PDF `README` for submission
- A linkable citation/BibTeX block for academic use
```

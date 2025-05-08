# 🧠 Sketch-to-Image Translation using CycleGAN & Pix2Pix

A Deep Learning project aimed at translating sketches into photorealistic images using two powerful GAN architectures — CycleGAN (for unpaired datasets) and Pix2Pix (for paired datasets). This project demonstrates the effectiveness of GANs in fashion design visualization and face reconstruction from sketch inputs.

## 👨‍💻 Team Members
- Manjur Kovadiya
- Rushiraj Jadeja
- Vandan Patel

---

## 🎯 Objective

- Translate raw sketches into realistic images for fashion and facial datasets.
- Compare the performance of CycleGAN and Pix2Pix on unpaired vs paired datasets.
- Visualize improvements over training using loss plots and output snapshots.

---

## 📦 Dataset Overview

### Fashion Dataset:
- Contains *paired* and *unpaired* sketch-real image sets.
- Images resized to **256x256** pixels.
- Split into `train/val` folders.

### Face Dataset:
- Contains *paired* sketch-real image sets.
- Stored in a single folder.
- Images resized to **256x256** pixels.

---

## 🔧 Model Architectures

### CycleGAN
- 2 Generators: `G_S→R`, `G_R→S`
- 2 Discriminators: `D_S`, `D_R`
- Losses: **Adversarial + Cycle-Consistency + Identity**
- Suitable for **unpaired** data

### Pix2Pix
- Single Generator and Discriminator
- Requires **paired** images
- Uses **U-Net** architecture and PatchGAN

---

## 🧪 Training Details

- **Optimizer**: Adam (lr=0.0001, β1=0.5, β2=0.999)
- **Loss Functions**: MSE, L1
- **Early Stopping**: Enabled for stability
- **Output Generation**: Every 5 epochs
- **Replay Buffer**: Used in Discriminator training to reduce oscillations

---

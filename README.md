🧠 Sketch-to-Image Translation using CycleGAN & Pix2Pix

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


## 📈 Results

- Models show significant improvement over epochs
- CycleGAN learns structure via cycle-consistency
- Pix2Pix generates more accurate outputs when paired data is available

<img width="596" alt="image" src="https://github.com/user-attachments/assets/f3d32609-403c-44d1-be9b-ec78441ead04" />#

---

## 🔍 Future Work

- Improve realism using FID (Fréchet Inception Distance)
- Apply better architectures (e.g., StyleGAN2, SPADE)
- Extend to other domains like architecture or product design

---

## 🏁 Conclusion

We successfully demonstrated sketch-to-image translation using CycleGAN and Pix2Pix. The models were able to generate realistic outputs from limited data and offer a foundation for future research and product development in creative AI.

---

## 📬 Contact

For any queries or collaborations, feel free to reach out to:

**Manjur Kovadiya**  
[LinkedIn](https://www.linkedin.com/in/manjur-kovadiya/) | [Email](mailto:kovadiyamanjur@gmail.com)

---

⭐ Don't forget to star this repo if you find it useful!

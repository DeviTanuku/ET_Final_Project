# 🎨 AI-Based Image Colorization with Pix2Pix GAN

> 🧠 **Course:** Emerging Technologies in AI  
> 📘 **Project Type:** Final Project  
> 👥 **Authors:** Antra Nayudu, Kartik Kalra, Devi Tanuku  
> 🖼️ **Focus:** Bringing black-and-white photos to life using deep learning  

---

## 📝 Project Description

This project uses a deep learning approach to colorize black-and-white images. We implemented a **Pix2Pix Conditional GAN** trained on the **DIV2K dataset**, enabling automatic generation of realistic, vivid color images from grayscale inputs. The system aims to assist in art restoration, historical preservation, and digital media production. It balances color accuracy, structure preservation, and fine detail generation.

---

## 🎯 Objectives

- Automatically colorize grayscale images using a deep generative model
- Preserve fine structural details and generate realistic colors
- Evaluate model performance using both qualitative and quantitative metrics
- Address practical use cases in digital art, film restoration, and archives

---

## 📊 Dataset

- **Source:** [Kaggle - DIV2K Dataset](https://www.kaggle.com/datasets/ambarish/div2k)  
- **Content:** Over 800 high-resolution PNG images including landscapes, portraits, monuments, and everyday objects  
- **Preprocessing Steps:**
  - Image cleanup and resolution standardization
  - Normalization (pixel values scaled to [0,1])
  - Data augmentation (flips, rotations)
  - Splitting into train/val/test (80/10/10)

---

## 🧱 Model Architecture

- **Model Type:** Pix2Pix GAN  
- **Generator:** U-Net with skip connections  
- **Discriminator:** PatchGAN  
- **Loss Functions:**
  - L1 Loss (pixel-wise similarity)
  - Binary Crossentropy (realism evaluation)  
- **Optimizer:** Adam (lr = 2e-4, β₁ = 0.5)

---

## 🧪 Evaluation Metrics

- **PSNR (Peak Signal-to-Noise Ratio):** Measures pixel-level accuracy
- **SSIM (Structural Similarity Index):** Measures perceptual similarity
- **FID (Frechet Inception Distance):** Measures realism by comparing feature distributions
- **Result Snapshot:**  
  - SSIM ≈ 0.61  
  - PSNR ≈ 21.3 dB  
  - FID decreases as training progresses

---

## 📂 Repository Structure

AI_Colorization_Project/ ├── 📓 DeviSriSwetha_Tanuku_Assignment2.ipynb # Jupyter notebook with full model pipeline ├── 📄 DeviSriSwetha_Tanuku_Assignment2_presentation.pdf # Final project slides ├── 📄 DeviSriSwetha_Tanuku_Assignment1_FinalProjectProposal.pdf # Initial project proposal ├── 📄 ET_Report.pdf # Detailed technical report ├── 📁 output_images/ # Sample results from the trained model │ ├── epoch_100_sample1.png │ ├── epoch_100_sample2.png │ └── ... ├── 📄 requirements.txt # Python dependencies └── 📄 README.md # This file

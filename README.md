# GANS
# GAN Implementations for Learning

This repository contains implementations of various Generative Adversarial Networks (GANs). Each folder corresponds to a specific GAN architecture, implemented as part of a personal project to understand and explore the fundamental concepts and practical applications of GANs.

## Project Structure

GAN-Implementations/ ├── 1. SimpleGAN/ # A basic implementation of GANs ├── 2. DCGAN/ # Deep Convolutional GAN ├── 3. WGAN/ # Wasserstein GAN ├── 4. WGAN-GP/ # Wasserstein GAN with Gradient Penalty ├── CycleGAN/ # GAN for image-to-image translation ├── ESRGAN/ # Enhanced Super-Resolution GAN ├── Pix2Pix/ # Paired image-to-image translation ├── ProGAN/ # Progressive Growing GAN ├── SRGAN/ # Super-Resolution GAN ├── StyleGAN/ # Style-based GAN for high-quality image generation

yaml
Copy code

## Details of Each GAN

### **1. SimpleGAN**
A minimal implementation of the original GAN architecture to understand the core principles of adversarial training.

- **Key Features**: Simple generator and discriminator.
- **Use Case**: Learning the basic dynamics between the generator and discriminator.

---

### **2. DCGAN (Deep Convolutional GAN)**
A GAN implementation that uses convolutional layers to generate realistic images.

- **Key Features**: Convolutional and transposed convolutional layers, batch normalization, and LeakyReLU activation.
- **Use Case**: Generating images of a specific domain (e.g., MNIST, CIFAR-10).

---

### **3. WGAN (Wasserstein GAN)**
A GAN variant that uses the Wasserstein distance to address mode collapse and improve training stability.

- **Key Features**: Wasserstein loss function, weight clipping.
- **Use Case**: Stable training for high-quality image generation.

---

### **4. WGAN-GP (Wasserstein GAN with Gradient Penalty)**
An improvement over WGAN that introduces a gradient penalty for more stable training.

- **Key Features**: Gradient penalty instead of weight clipping.
- **Use Case**: Overcomes limitations of WGAN by providing smoother convergence.

---

### **CycleGAN**
A GAN for unpaired image-to-image translation.

- **Key Features**: Cycle-consistency loss, two generators and two discriminators.
- **Use Case**: Style transfer (e.g., transforming horses to zebras or summer to winter).

---

### **ESRGAN (Enhanced Super-Resolution GAN)**
A GAN for generating high-resolution images from low-resolution inputs.

- **Key Features**: Residual-in-Residual Dense Blocks, perceptual loss.
- **Use Case**: Image super-resolution tasks.

---

### **Pix2Pix**
A GAN for paired image-to-image translation.

- **Key Features**: Conditional GAN (cGAN), paired training data.
- **Use Case**: Image-to-image translation tasks like edge-to-photo.

---

### **ProGAN (Progressive Growing GAN)**
A GAN that grows progressively during training to generate high-resolution images.

- **Key Features**: Progressive layer addition, fade-in transitions.
- **Use Case**: Training GANs for high-resolution image synthesis.

---

### **SRGAN (Super-Resolution GAN)**
A GAN for super-resolution tasks.

- **Key Features**: Uses perceptual loss and adversarial loss for high-quality results.
- **Use Case**: Upscaling images to higher resolutions.

---

### **StyleGAN**
A GAN that generates high-quality images with control over style and features.

- **Key Features**: Style mixing, AdaIN (Adaptive Instance Normalization).
- **Use Case**: Generating realistic and diverse images, such as human faces.

---

## Requirements

- Python 3.8+
- Common deep learning libraries such as TensorFlow or PyTorch.
- Additional requirements for each GAN are listed in their respective folders.

To install general dependencies, run:
```bash
pip install -r requirements.txt
Usage
Each folder contains:

A README.md or notebook explaining the implementation.
Code for training and testing the GAN.
Pre-trained models or checkpoints (if applicable).
To train a specific GAN:

Navigate to its folder.
Run the training script:
bash
Copy code
python train.py
To test or generate samples:

bash
Copy code
python generate.py
Refer to individual folders for specific instructions.
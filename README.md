🎨 Image Colorization using GANs

AI-powered image colorization project that converts grayscale landscape images into realistic colored images using a Generative Adversarial Network (GAN) built with TensorFlow/Keras.
The model learns color distributions from real-world landscape images and generates plausible colorized outputs from grayscale inputs.


🚀 Project Overview
This project uses a Generator–Discriminator GAN architecture for automatic image colorization.
The Generator takes a grayscale image as input and predicts a colored RGB image.
The Discriminator evaluates whether the generated image looks realistic compared to real color images.
The system is trained adversarially so the generator continuously improves its colorization quality.

🛠️ Tech Stack
Python
TensorFlow / Keras
NumPy
Matplotlib
Google Colab
GAN Architecture

📂 Dataset
Landscape image dataset
Total Images: 7129
Image Size: 128 × 128
Separate grayscale and color image folders


🧠 Model Architecture
Generator Network
Encoder–Decoder CNN architecture using:
Conv2D layers
Batch Normalization
Conv2DTranspose layers
Tanh activation for RGB output generation
Discriminator Network
CNN-based classifier that distinguishes:
Real colored images
GAN-generated images


🖼️ Output Visualization

The model generates:
Input grayscale image
GAN-colorized output
Original ground-truth image
This allows direct visual comparison between generated and actual colors.

📊 Features
Automatic grayscale-to-color conversion
Deep learning based GAN implementation
Image preprocessing pipeline
TensorFlow data pipeline with prefetching
Real-time result visualization
GPU accelerated training support

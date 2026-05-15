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
⚙️ Training Details
Parameter	Value
Epochs	40
Batch Size	16
Optimizer	Adam
Learning Rate	2e-4
Beta_1	0.5
Loss Function	Binary Crossentropy + L1 Loss
📈 Training Results

The GAN successfully learned realistic color mappings for landscape images over 40 epochs.

Example Loss Logs
Epoch 1/40  | G: 12.5864 | D: 1.0049
Epoch 10/40 | G: 10.2620 | D: 0.6365
Epoch 20/40 | G: 10.2686 | D: 0.5996
Epoch 40/40 | G: 9.5857  | D: 0.6079
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
📁 Project Structure
├── dataset/
│   ├── gray/
│   └── color/
│
├── train.py
├── generator.py
├── discriminator.py
├── utils.py
├── results/
└── README.md
▶️ How to Run
1️⃣ Clone Repository
git clone https://github.com/yourusername/image-colorization-gan.git
cd image-colorization-gan
2️⃣ Install Dependencies
pip install tensorflow matplotlib numpy
3️⃣ Run Training
python train.py
🔥 Future Improvements
Add U-Net based generator
Train on higher resolution images
Deploy as a web application
Add attention mechanisms
Improve color consistency
Support video colorization
💡 Learning Outcomes

Through this project, I learned:

GAN training workflows
Image preprocessing pipelines
Adversarial loss optimization
CNN encoder-decoder architectures
TensorFlow dataset optimization
Deep learning model debugging

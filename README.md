AI Image Caption Generator

An AI-powered image captioning web app built using Streamlit and a pretrained DenseNet201 model.
This project automatically generates meaningful text captions for images — describing what it "sees" in natural language.

Features

Uses DenseNet201 as the pretrained CNN backbone for feature extraction.

Generates human-like captions for any image.

Interactive and simple Streamlit web interface.

Real-time predictions with quick processing.

Upload your own images to see AI-generated captions instantly.

Model Overview

The model combines:

DenseNet201 (pretrained on ImageNet) to extract rich visual features from the input image.

LSTM or Transformer-based decoder to convert extracted features into descriptive text sequences.

The model has been trained or fine-tuned on an image-caption dataset such as MS COCO (or your custom dataset).

Tech Stack

Python 3.9+

TensorFlow / Keras

Streamlit

NumPy, Pandas

Pillow (for image processing)

Installation and Usage
1. Clone this repository
git clone https://github.com/bunny182005/image_captioning.git
cd image-caption-generator

2. Install dependencies
pip install -r requirements.txt

3. Run the Streamlit app
streamlit run main.py

4. Upload an image

Once the app launches in your browser, upload an image.
The model will analyze it and display a generated caption below.

Project Structure
├── main.py                # Streamlit app entry point
├── model/
│   ├── densenet201_model.h5   # Trained model file (if applicable)
│   └── tokenizer.pkl          # Tokenizer for text generation
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
└── assets/                # Sample images or screenshots

Example Output

Input Image: a man riding a horse on a beach
Generated Caption:

“A person riding a horse along the shore under a bright sky.”

Future Improvements

Add support for multiple caption styles (formal, creative, etc.).

Integrate multilingual caption generation.

Improve inference speed with model optimization and quantization.

License

This project is released under the MIT License — free to use, modify, and share.

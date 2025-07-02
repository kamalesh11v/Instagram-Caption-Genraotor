This project aims to bridge the gap between computer vision and natural language processing by generating textual descriptions of images. Given an image, the system generates a caption that describes the contents and context of the image.

📈 Project Pipeline
Data Preprocessing

Load and clean image captions.

Tokenize and pad caption text.

Extract image features using a pre-trained CNN (like InceptionV3 or VGG16).

Model Building

Combine CNN-extracted image features and tokenized captions.

Use an LSTM-based decoder for caption generation.

Training

Use categorical cross-entropy loss.

Implement early stopping and checkpointing.

Prediction

Input an image.

Extract its features.

Generate a caption word by word.

📂 Dataset
Source: Flickr8k/Flickr30k/MSCOCO

Contains images and corresponding captions.

Image captions cleaned by removing punctuation, lowercasing, and tokenizing.

🛠️ Technologies Used
Python 3.x

TensorFlow / Keras

NumPy

Pandas

Matplotlib / Seaborn (for visualization)

NLTK (for text preprocessing)

Pre-trained CNN models (InceptionV3 / VGG16)

Jupyter Notebook / Google Colab

🖥️ Model Architecture
CNN Encoder: Pre-trained InceptionV3 model (without final classification layer) to extract a 2048-dimensional feature vector from each image.

RNN Decoder: LSTM-based model

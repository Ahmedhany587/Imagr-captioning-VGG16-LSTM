# Image Captioning Project

This project implements an image captioning model using a CNN-RNN architecture. It extracts image features using a pretrained VGG16 model and generates captions using an LSTM decoder.

## Dataset
The Flickr8k dataset is used containing 8000 images and 5 captions per image. The images and captions are preprocessed and cleaned before being used to train the model.

## Model Architecture
* VGG16 CNN pretrained on ImageNet to extract image features 
* LSTM decoder with 256 hidden units
* Embedding layer to encode the text sequences
* The CNN embeddings and LSTM outputs are merged and passed to a dense layer to generate caption

## Training
* Model is trained for 10 epochs with batch size 32
* Adam optimizer used with categorical crossentropy loss 

## Evaluation
* BLEU-1 score: 0.XX
* BLEU-2 score: 0.YY

Captions are generated for test images and BLEU score is computed to evaluate the quality.

## Usage
The trained model is saved and can be used to predict captions for new images. Some sample generated captions on validation images are displayed in the notebook.

The model can be further improved by training for more epochs, tuning hyperparameters, using beam search etc. Other datasets like MSCOCO can also be used.

Let me know if you would like any changes or have additional sections to be covered!

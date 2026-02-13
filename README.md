# Image Captioning System using CNN–LSTM
## Overview

This project implements an end-to-end image captioning system that automatically generates natural language descriptions for images using deep learning. The system follows a classical encoder–decoder architecture combining convolutional neural networks for visual understanding and recurrent neural networks for language generation.

 ## Architecture

- Encoder: Pre-trained VGG16 CNN used to extract high-level visual features from images

- Decoder: LSTM-based sequence model to generate captions word-by-word

- Training Strategy: Teacher forcing for stable and faster convergence

- Inference Optimization: Top-k sampling to reduce repetitive and generic captions

## Model Flow Diagram
<img width="2000" height="1125" alt="image" src="https://github.com/user-attachments/assets/f728cccf-9114-49a0-a1db-9b913b8dc930" />

## Evaluation

Model performance is evaluated using BLEU scores (BLEU-1 to BLEU-4) along with qualitative inspection of generated captions. The system effectively captures objects, scene context, and basic attributes, producing grammatically correct and meaningful descriptions.

## Limitations

- Limited recognition of complex or dynamic actions

- Inaccurate object counting due to lack of explicit detection mechanisms

- No attention mechanism, leading to reduced region-specific focus

- Dataset bias affecting caption diversity and higher-order BLEU scores

## Future Enhancements

- Integrate attention mechanisms for improved visual focus

- Replace LSTM with Transformer-based decoders

- Explore multimodal models such as ViT, CLIP, or vision–language transformers

- Incorporate object detection to improve counting accuracy

## Tech Stack

Python, TensorFlow, Keras, CNN, LSTM, VGG16, Natural Language Processing (NLP), BLEU Score, NumPy, Matplotlib

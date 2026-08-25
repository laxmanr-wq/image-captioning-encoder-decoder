# Image-Captioning-Encoder-Decoder

The CNN (likely a pre-trained model like ResNet) is used to encode the images into feature vectors.

The LSTM decoder then takes these feature vectors and generates captions, word by word.

ViT (Vision Transformer) Encoder: The Vision Transformer is used to process and encode images into feature vectors. This model is specifically designed for image understanding tasks.

GPT-2 Decoder: GPT-2, a transformer-based language model, is used to generate captions based on the encoded image features. The tokenizer is customized to include special tokens for the beginning and end of the sequence.

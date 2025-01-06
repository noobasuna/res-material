# Resnet-like Architecture for Toughness Prediction for Self-Healing Material
## Overview

We advance this with a residual neural network (ResNet) architecture, to show that the proposed solution is generalized across different models. We chose ResNet because it is a lightweight feature extraction model often used in various tasks and is an advancement from the more conventional CNN. For this tailored model, only 400 epochs were performed to prevent overfitting, which also demonstrates the lower computational cost compared to the baseline CNN model.

The baseline CNN architecture was enhanced by designing a custom variant of ResNet. 
While maintaining the core concept of residual learning from the original ResNet architecture, our customization introduces several key modifications: (1) the input layer is adapted to process grayscale images of dimension 160 x 100 x 1, diverging from the standard ResNet-18's 224 x 224 x 3 RGB input; (2) the residual block structure is simplified to six blocks with a progressive filter expansion (64 --> 128 --> 256 filters), compared to the conventional ResNet-18's deeper architecture; and (3) the final classification layers are tailored with additional dense layers (128 and 64 units) incorporating L2 regularization to prevent overfitting, replacing the traditional fully connected layer structure. These modifications were specifically designed to balance the model's capacity with the complexity of our toughness prediction task while maintaining the advantages of residual learning for gradient flow during training.

## Contact
For any inquiries, please contact at tan.peisze@monash.edu.

# Vanilla-Decoder
 
This repository contains the implementation of a **Vanilla Transformer Decoder Block** built using **PyTorch**. It can generate text based on a training corpus and has the following main components:
- **Multi-Head Attention**
- **FeedForward Neural Network**
- **Layer Normalization**

## Features
- Tokenizes the input text and processes it using embeddings.
- Utilizes a multi-layered transformer architecture with self-attention and feedforward networks.
- Can generate text tokens one-by-one using the trained model.
- Performs loss computation based on the cross-entropy between predicted and actual tokens.

## Model Architecture
- **Embedding**: Each character is embedded into a continuous vector space.
- **Multi-Head Attention**: Attention mechanism with multiple heads to focus on different parts of the sequence.
- **FeedForward Network**: Fully connected layers used to process intermediate states.
- **Positional Encoding**: Adds positional information to the token embeddings.
- **Layer Normalization**: Normalizes the intermediate outputs to ensure stable training.

## Training Configuration
- **Batch Size**: `64`
- **Block Size**: `256` (length of input sequence)
- **Learning Rate**: `3e-4`
- **Number of Layers**: `6`
- **Number of Attention Heads**: `6`
- **Dropout Rate**: `0.2`
- **Evaluation Interval**: `500`

### Steps to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Pragateeshwaran/Vanilla-Decoder.git
   cd Vanilla-Decoder
   ```

2. **Install dependencies**:
   ```bash
   pip install torch
   ```

3. **Prepare the training data**:
   - Ensure you have a `data.txt` file in the repository directory. This file contains the text corpus for training.

4. **Run the training script**:
   ```bash
    Run All cells in Jupyter Notebook
   ```

5. **Generate text**:
   After training, the model can generate text using the `generate` function in the model.

### Example Output
```
My lord of state, if he are not more but toucher
Than in Juniusal by a boar, the instructor...
```  

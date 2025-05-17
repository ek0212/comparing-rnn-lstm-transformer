This repository provides a simple, hands-on exploration of how three fundamental neural network architectures—RNN (Recurrent Neural Network), LSTM (Long Short-Term Memory), and Transformer (Self-Attention)—process and "remember" sequences. The code is designed as an educational demo, with rich print statements and analogies, to help you intuitively understand the mechanics of each model.

## Overview

- **Goal:**  
  Compare how RNNs, LSTMs, and Transformers process a short sequence (`'a b c'`), emphasizing their differences in memory and attention.
- **Approach:**  
  All models use randomly initialized weights and a tiny 3-token vocabulary. This is for demonstration only; no training is performed.

## What’s Inside

- **Jupyter Notebook:**  
  The main code is in [`comparing_rnn_lstm_transformer.ipynb`](comparing_rnn_lstm_transformer.ipynb).
- **Code Structure:**  
  - **Setup:** Imports, random seed, vocabulary, and embeddings.
  - **RNN Section:**  
    - Step-by-step processing with a basic hidden state.
    - Shows how information is carried forward (or forgotten).
  - **LSTM Section:**  
    - Adds gated memory mechanisms (input, forget, output gates).
    - Demonstrates how LSTM can better manage long-term dependencies.
  - **Transformer Section:**  
    - Implements self-attention over the entire sequence.
    - Shows how each token attends to all others in parallel.
  - **Summary:**  
    - Recaps the core differences and analogies for each model.

## Requirements

- Python 3.x
- PyTorch
- NumPy

Install dependencies with:
```bash
pip install torch numpy
```

## Running the Demo

1. Open [`comparing_rnn_lstm_transformer.ipynb`](comparing_rnn_lstm_transformer.ipynb) in Jupyter Notebook or JupyterLab.
2. Run the notebook cells in order.
3. Read the detailed print outputs and comments to follow along with each step.

## Learnings

- **RNN:** Reads input sequentially, carries information forward in a single hidden state, but struggles with long-term memory.
- **LSTM:** Adds gates to manage memory more intelligently, mitigating the “forgetfulness” problem.
- **Transformer:** Uses self-attention to view the entire sequence at once, allowing for richer context and parallel computation.

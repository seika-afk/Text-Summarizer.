# 📝 Text Summarizer

This project implements a **Text Summarization model** using a **Sequence-to-Sequence LSTM architecture** with an encoder-decoder setup in TensorFlow/Keras. It summarizes long pieces of text into concise summaries.
- Encoder-Decoder architecture with stacked LSTM layers.
- Preprocessing with padding and tokenization.
- Custom inference decoding loop using greedy search.
- Training with teacher forcing.
- Optional support for saving/loading model weights.

##  Model Architecture
- **Embedding layers** for encoder and decoder inputs.
- **3-layer stacked LSTM encoder** for rich context learning.
- **1-layer LSTM decoder** initialized with encoder states.
- **TimeDistributed Dense Softmax layer** for output token prediction.

##  Dependencies
- Python - TensorFlow / Keras
- Pandas
- scikit-learn

## How to Use
1. Review the last line from the notebook.

## 📈 Output
Predicts one-line summaries for long input texts.  
Example:
> Input: "The government announced new education policies..."  
> Output: `"government launches education reforms"`

### Side Note
- During Training and hypertuning ,i ran out of tpu from google collab, so couldnt train more,
- but The last i tried The metrics were like this :

- - accuracy : 75%
  - loss : 1.3

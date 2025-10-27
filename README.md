# 🔄 RNN Deep Learning Projects

A collection of Recurrent Neural Network implementations for natural language processing tasks using PyTorch and TensorFlow/Keras.

## 📁 Projects

### 1. 🌍 Seq2Seq Translation Model (PyTorch)
English-to-French neural machine translation using encoder-decoder architecture with LSTM.

**Features:**
- Encoder-Decoder architecture with LSTM layers
- Teacher forcing mechanism
- Custom vocabulary building and tokenization
- Special tokens handling (PAD, SOS, EOS, UNK)

**Quick Start:**
```bash
python "Seq2Seq traduction model with PyTorch.py"
```

---

### 2. 🎭 Sentiment Analysis Comparison (TensorFlow/Keras)
Compare three RNN architectures (SimpleRNN, LSTM, GRU) on IMDB movie reviews sentiment classification.

**Features:**
- Three model architectures: SimpleRNN, LSTM, GRU
- IMDB dataset (25,000 movie reviews)
- Performance comparison and visualization
- Binary sentiment classification (positive/negative)

**Quick Start:**
```bash
python "RNN Project Sentiment Analysis.py"
```

## 🔧 Requirements

```bash
# For Seq2Seq project
pip install torch numpy

# For Sentiment Analysis project
pip install tensorflow keras matplotlib
```

## 📊 Expected Results

**Translation Model:**
- Input: "good night"
- Output: "bonne nuit"

**Sentiment Analysis:**
- SimpleRNN: ~80-85% accuracy
- LSTM: ~85-88% accuracy
- GRU: ~85-88% accuracy

## 🧠 Key Concepts

| Concept | Description |
|---------|-------------|
| **Seq2Seq** | Encoder compresses input → Decoder generates output |
| **LSTM** | Handles long-term dependencies with gates |
| **GRU** | Simplified LSTM with fewer parameters |
| **Teacher Forcing** | Uses ground truth as decoder input during training |
| **Embeddings** | Dense vector representations of words |

## 📈 Architecture Overview

### Seq2Seq Model
```
Input Sequence → [Encoder LSTM] → Hidden State → [Decoder LSTM] → Output Sequence
```

### Sentiment Analysis Models
```
Text → [Embedding] → [RNN/LSTM/GRU] → [Dense] → Sentiment (0/1)
```

## 🚀 Usage Examples

**Translation:**
```python
sentence = "hello"
translation = translate_sentence(model, sentence, english_vocab, french_vocab, max_len_fr, device)
# Output: "bonjour"
```

**Sentiment Analysis:**
```python
# Models are trained and evaluated automatically
# Training graphs show accuracy comparison across architectures
```

## 📚 Datasets

- **Translation**: Custom English-French parallel corpus (5 sentence pairs)
- **Sentiment Analysis**: IMDB movie reviews (50,000 reviews)

## 🎯 Learning Objectives

- Understanding RNN architectures and their variants
- Implementing sequence-to-sequence models
- Comparing SimpleRNN, LSTM, and GRU performance
- Working with text preprocessing and embeddings
- Handling sequential data in deep learning

## 🤝 Contributing

Feel free to:
- Add more language pairs for translation
- Experiment with attention mechanisms
- Try bidirectional RNNs
- Implement beam search for better translations

## 📄 License

MIT License

---

**⭐ Star this repo if you find it useful for learning RNNs!**

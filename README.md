#  Sequence-to-Sequence Transliteration — English → Hindi

This project implements **character-level neural sequence-to-sequence models** for transliterating **Indian names** from English to Hindi.  
It explores and compares **RNN (GRU)** and **GRU + Attention** architectures, evaluating translation quality using BLEU metrics and decoding strategies.

---

## 🚀 Features
- Implemented **Encoder–Decoder GRU** model for character-level transliteration.  
- Extended with **Bahdanau Attention**, improving alignment and contextual mapping.  
- Integrated both **greedy** and **beam-search decoding** for output sequence generation.  
- Achieved **BLEU score = 0.73** with Attention + Beam Search — significantly outperforming the vanilla GRU baseline.  
- Visualized attention weights to interpret input–output alignment.

---

## 🧩 Dataset
- **Indian name transliteration dataset** (English–Hindi pairs).  
- Preprocessed to handle Unicode normalization and tokenization at character level.  
- Split into **training / validation / test** sets for model evaluation.

---

## 🧠 Models Implemented
| Model | Architecture | Decoding | BLEU |
|--------|---------------|----------|------|
| GRU Encoder–Decoder | 1-layer GRU | Greedy | 0.65 |
| GRU + Attention | Bahdanau Attention | Beam Search | **0.73** |

---

## 📈 Results
- Attention-based model demonstrated **better sequence alignment** and reduced transliteration errors.  
- Beam Search decoding improved final output fluency and accuracy.  
- Attention visualizations revealed interpretable source-target mappings.

---

## 🛠️ Requirements
```bash
pip install torch numpy matplotlib tqdm

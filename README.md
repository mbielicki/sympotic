# sympotic

An AI poet and philosopher.

This is a small toy implementation of a decoder‑only Transformer (autoregressive language model) written as a Jupyter notebook (SympoticDOT.ipynb). It uses PyTorch + PyTorch Lightning to train a tiny language model on tokenized text from training.txt, logs training to TensorBoard, and contains simple inference routines to generate responses and conversational continuations.

# Tokens

It's vocabulary is limited to the following tokens:

```python
tokens = [
    '<EOS>', '.', '?', 'what', 'when',
    'so', 'to', 'for', 'of', 'and',
    'not', 'but', 'all', 'more',
    'it', 'you', 'I', 'me', 'that',
    'is', 'do', 'can', 'think', 'know', 'like', 'love', 'make', 'need',
    'happy', 'hard', 'food', 'good'
    ]
```

# Examples

User Input:
what is love ? <EOS>

Predicted Tokens:
I need to make you happy . <EOS>

---

User Input:
what is love ? <EOS>

Predicted Tokens:
I think of food . <EOS>

# Quotes

`I do not think . I think .`
`I can think I do not think .`
`you are good to me to think .`

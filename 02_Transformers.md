# # Transformer Architecture

- Most mordern LLMs rely on the transformer architecture.
- This deep neural newtwork architecture introduced in 2017 paper "**`Attention Is All You Need`**".
- Original tranformer is developed for **Machine translation**.
  - Ex : Translating english text to german and french

---

## # Simplified Transformer Architecture

Source : **Build a LLM from Scratch** (By - Sebastian Raschka)

<img src="https://github.com/user-attachments/assets/8c84d060-191e-486d-9684-9f97143c6b39" width="1000" height="600">

### Step-by-Step Flow

**1. `Input sentence`**
- The source text enters the model, for example: “This is an example”.

**2. `Preprocessing for encoder`**
- The input text is cleaned and converted into token IDs, then prepared for the encoder.
- Common preprocessing steps
  - Tokenization
  - Encoding
  - Padding

**3. `Encoder processes the input*`*
- The encoder reads the input and creates text encodings that capture meaning and context.
- Encoder Tasks
  - Understands meaning
  - Captures relationships between words
  - Produces encoded text representations

**4. `Embedding vector passed to decoder`**
- The encoder output becomes an embedding / context vector and is sent to the decoder.

**5. `Partial output text`**
- The decoder starts with an initial partial output, for example: “Das ist ein”.
- It predicts one word at a time.

**6. `Preprocessing for decoder`**
- The partial output text is also tokenized and prepared for the decoder input.
- The decoder uses:
  - Previous generated words
  - Encoder embeddings

**7. `Decoder generates translated text`**
- Using the encoder’s context and its own previous output, the decoder keeps generating the next words.
- The model predicts the next word repeatedly until the sentence is complete.

**8. `Complete output`**
- The final translated sentence is produced, for example: “Das ist ein Beispiel”.



### Overall Transformer Flow

```text
Input Text
     ↓
Preprocessing
     ↓
Encoder
     ↓
Embeddings / Encoded Vectors
     ↓
Decoder
     ↓
Output Layers
     ↓
Generated Text
```

---

## #  




















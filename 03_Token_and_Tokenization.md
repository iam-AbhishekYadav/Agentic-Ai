# # Token and Tokenization

## # What is Token ?

- A token is the smallest piece of text that an LLM (Large Language Model) processes.
- A token can be:
  - a word
  - part of a word
  - a single character
  - punctuation marks
  - spaces or symbols
- LLMs do not directly understand sentences.They first convert text into:
  - `Text → Tokens → Numbers (Token IDs) → Embeddings`


> Exapmle :
>
> "This is an example"
>
> **Possible tokens:**  
> ["This", "is", "an", "example"] &ensp;  **OR**  &ensp;  ["This", " is", " an", " example"]


## # What is Tokenization ?

- The process of breaking down sensitive data, text, or real-world assets into smaller, distinct, and manageable units called Tokens


## # Types of Tokenization

### 1. Word Tokenization
- Splits by words.

```
"I love AI"
→ ["I", "love", "AI"]
```

### 2. Character Tokenization
- Splits by characters.

```
"cat"
→ ["c", "a", "t"]
```

### 3. Subword Tokenization (used in LLMs)
- Splits into meaningful subwords.

```
"unhappiness"
→ ["un", "happy", "ness"]
```

> [!NOTE]  
> Modern LLMs mainly use:
> 
> - BPE (Byte Pair Encoding)
> - WordPiece
> - SentencePiece




































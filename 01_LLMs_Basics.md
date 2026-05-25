# Agentic Ai

# # What is a LLMS ?

- Neural network designed to understand, generate and respond to human like text.
- Deep nural networks trained on massive amount of text data.
- Large Language Models
  - **Large** : Models have billions of parameters.
  - **Lnaguage Models** : These models do a wide range of NLP tasks ; question answering, translation, sentiment analysis and much more.

## LLMs vs Earlier NLP Models

- LLMs : It can do wide range of NLP tasks.
- NLP : It is designed for specific tasks like language translation etc.
- Earlier language models could not write an email from custom instructions, a task that is trivial for modern, LLMs


## Applications of LLMs

- Chatbots & Virtual Assistants
- Machine translation
- Novel text generation
- Sentiment analysis

---

##  # LLM vs Gen Ai vs Ai vs DL vs ML vs NLP

<img src="https://github.com/user-attachments/assets/cd31fcd0-497e-4c3b-a2fe-29ed11a55260" width="800" height="600">

---

## # Pretraining vs Fine-tuning in LLMs

| Feature | Pretraining | Fine-tuning |
|---|---|---|
| Purpose | Teach the model general language understanding | Teach the model a specific task/domain |
| Data Used | Massive internet-scale text data | Smaller specialized dataset |
| Training Type | Learns patterns, grammar, facts, reasoning | Adjusts behavior for a task |
| Cost | Very expensive (huge GPUs + time) | Much cheaper and faster |
| Example | Training GPT models on web data | Fine-tuning for coding, medical, or chatbot tasks |
| Output | Base/Foundation model | Task-specialized model |

#### Simple Example
- **Pretraining:** Model learns “how language works.”
- **Fine-tuning:** Model learns “what specific job to do.”

#### Real-world Analogy
- **Pretraining = School education**
- **Fine-tuning = Job training/specialization**

---

## # Pretraining + Fine-tuning Schematic

```text
+---------------------------------------------------+
|                      DATA                         |
+---------------------------------------------------+
| • Internet text                                   |
| • Books                                            |
| • Media                                            |
| • Research articles                                |
+---------------------------------------------------+
| Raw unlabeled text → trillions of words           |
+---------------------------------------------------+

                         │
                         │ Train
                         ▼

+---------------------------------------------------+
|            PRETRAINED LLM (Foundation Model)      |
+---------------------------------------------------+
| • Trained on massive unlabeled text data          |
| • Learns basic language capabilities              |
| • Understands patterns, grammar, reasoning        |
+---------------------------------------------------+

                         │
                         │ Further Train
                         ▼

                 +----------------------+
                 |   Labeled Dataset    |
                 +----------------------+

                         │
                         ▼

+---------------------------------------------------+
|                 FINE-TUNED LLM                    |
+---------------------------------------------------+
| Trained on labeled datasets for specific tasks    |
|                                                    |
| • Classification                                   |
| • Summarization                                    |
| • Translation                                      |
| • Personal Assistant                               |
+---------------------------------------------------+
```

---

## # Steps for Building a LLM

### Step-1
- Train on a Large Corpus of Text Data (Raw Text)
- Raw Text : Raw text means regular text without any labeling information.
- Examples of Raw Text Data
  - Internet text
  - Books
  - Articles
  - Media content
  - Research papers

```text
Raw Text Data
      ↓
Training
```

### Step-2
- The first training stage of an LLM is called **Pretraining**.
- **Goal** : Create an initial pretrained LLM  (Base / Foundational Model)
- Example
  - GPT-3 is a pretrained model.
  - It is capable of text completion and next-word prediction.
- Capabilities of a Pretrained LLM
  - Predicting next words
  - Understanding language patterns
  - Basic reasoning
  - General language understanding

```text
Raw Unlabeled Text
        ↓
Pretraining
        ↓
Pretrained / Foundation LLM
```

### Step-3
- After obtaining the pretrained LLM, we can further train it using labeled datasets.
- This process is called Fine-tuning

```text
Pretrained LLM
        ↓
Training on Labeled Data
        ↓
Fine-tuned LLM
```

### Step-4
- There are two Popular Categories of Fine-tuning
  - Instruction Fine-tuning
  - Fine-tuning for Classification Tasks

1. Instruction Fine-tuning

- Labeled dataset consist of Instruction-answer pairs
- Examples
  - Text translation
  - Chat assistants
  - Airline customer support

```text
Instruction + Answer Pairs
            ↓
Instruction Fine-tuning
```

2. Fine-tuning for Classification Tasks

- Labeled dataset consist of text with associated labels
- Examples
  - Email → Spam / Not Spam
  - Review → Positive / Negative
  - News → Sports / Politics

### Example Format

```text
Text + Labels
      ↓
Classification Fine-tuning
```


### Overall Flow

```text
Raw Text Data
      ↓
Pretraining
      ↓
Pretrained / Foundation LLM
      ↓
Fine-tuning on Labeled Data
      ↓
Task-Specific Fine-tuned LLM
```



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


## LLM vs Gen Ai vs Ai vs DL vs ML vs NLP

<img src="https://github.com/user-attachments/assets/cd31fcd0-497e-4c3b-a2fe-29ed11a55260" width="800" height="600">

## Pretraining vs Fine-tuning in LLMs

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


## Pretraining + Fine-tuning Schematic

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

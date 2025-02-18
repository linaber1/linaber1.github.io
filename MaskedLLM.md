A masked language model (MLM) is a type of large language model (LLM) that learns to predict missing words in a sentence. This technique is commonly used in training transformer-based models like BERT (Bidirectional Encoder Representations from Transformers).
How Does a Masked LLM Work?
Masking Words:
Some words in a sentence are randomly replaced with a special "[MASK]" token.
Example:
Original sentence: "The cat sat on the mat."
Masked version: "The [MASK] sat on the mat."
Prediction:
The model is trained to guess the missing word based on the surrounding words.
Example output: "The cat sat on the mat."
Training Objective:
The model improves by adjusting its predictions based on how accurately it fills in the masked words over millions of examples.
Why Use Masked LLMs?
Understanding Context in Both Directions: Unlike older models that predict words only from left to right (like GPT models), masked LLMs consider context from both directions (left and right).
Better for NLP Tasks: This makes masked models highly effective for tasks like question answering, sentence completion, and text classification.
Examples of Masked LLMs
BERT (Bidirectional Encoder Representations from Transformers)
RoBERTa (a more refined version of BERT)
DistilBERT (a smaller, faster version of BERT)

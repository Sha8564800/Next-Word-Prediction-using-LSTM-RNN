# Next Word Prediction using LSTM

An NLP-based Deep Learning project that predicts the next word in a sequence using a Long Short-Term Memory (LSTM) neural network.

The model is trained on William Shakespeare's *Hamlet* and deployed as an interactive Streamlit web application.

---

##  Project Overview
Next Word Prediction is a Natural Language Processing (NLP) task where a model learns the patterns and relationships between words in a text corpus and predicts the most probable word that should come next.

For example:

**Input:**
> To be or not to

**Predicted Next Word:**
> be

This project uses an LSTM-based neural network to learn sequential patterns from Shakespeare's *Hamlet*.

---

## Objectives

- Process and tokenize Shakespeare's text.
- Convert text into numerical word sequences.
- Generate input-output training sequences.
- Train an LSTM-based language model.
- Predict the next word from a given sequence.
- Save the trained model and tokenizer.
- Deploy the application using Streamlit.

---

## Dataset

The model is trained using:

**Dataset:** Shakespeare's *Hamlet*

The text corpus contains approximately 4,818 unique tokens after tokenization.

The dataset was obtained using the NLTK Gutenberg corpus.


---

## LSTM Model Architecture

Input Sequence
      ->
Embedding Layer
100-dimensional embeddings
      ->
LSTM 150 units
      ->
Dropout 0.2
      ->
LSTM
200 units
      ->
Dense 4818 neurons
      ->
Softmax
      ->
Predicted Next Word


---

## Model Compilation
The model is compiled using:

Optimizer: Adam
Loss Function: Categorical Cross-Entropy
Evaluation Metric: Accuracy
Final Training Accuracy:82.7%
Highest Observed Training Accuracy:82.94%
Training Loss ≈ 0.6727
Training Accuracy ≈ 82.70%
Validation Loss ≈ 16.7293


---

## Model Deployment

The trained LSTM model has been deployed using Streamlit.
The application provides an interactive interface where users can enter a sequence of words and receive the predicted next word.



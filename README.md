# Next Word Prediction using RNN (Deep Learning)

## 📌 Project Overview

This project demonstrates a **Next Word Prediction system** using **Natural Language Processing (NLP)** and **Deep Learning**.
The model learns patterns from a given text dataset and predicts the **next possible word** in a sentence.

The model is trained using the popular nursery rhyme **"Twinkle Twinkle Little Star"** and predicts the next word based on the input sequence.

Example:

Input:
twinkle twinkle

Output:
twinkle twinkle little

---

## 🧠 Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* NLP (Natural Language Processing)
* RNN (Recurrent Neural Network)

---

## 📂 Project Structure

```
Next-Word-Prediction/
│
├── next_word_prediction_project.py
├── Next_word_prediction_project.ipynb
└── README.md
```

---

## ⚙️ Model Architecture

The project uses a **Recurrent Neural Network (RNN)** with the following layers:

* **Embedding Layer** – Converts words into dense vector representations
* **SimpleRNN Layer** – Learns sequential relationships in text
* **Dense Layer (Softmax)** – Predicts probability of the next word

Example model architecture:

```python
model = Sequential()
model.add(Embedding(input_dim=total_words, output_dim=10, input_length=max_seq_len-1))
model.add(SimpleRNN(64))
model.add(Dense(total_words, activation='softmax'))
```

---

## 🔄 How the Model Works

1️⃣ Convert text into lowercase

2️⃣ Tokenize the words using **Keras Tokenizer**

3️⃣ Create **n-gram sequences**

Example:

```
twinkle
twinkle twinkle
twinkle twinkle little
twinkle twinkle little star
```

4️⃣ Pad sequences to equal length

5️⃣ Train RNN model

6️⃣ Predict next word using trained model

---

## ▶️ How to Run the Project

### Step 1: Install dependencies

```
pip install tensorflow numpy
```

### Step 2: Run the Python file

```
python next_word_prediction_project.py
```

---

## 🧪 Example Predictions

Input:

```
twinkle twinkle
```

Output:

```
twinkle twinkle little
```

Input:

```
like a diamond
```

Output:

```
like a diamond in the sky
```

---

## 🎯 Features

✔ Text preprocessing using Tokenizer
✔ Sequence generation using n-grams
✔ Word embeddings using Embedding layer
✔ Sequence learning using RNN
✔ Next word prediction

---

## 🚀 Future Improvements

* Use **LSTM or GRU** instead of SimpleRNN
* Train on larger datasets
* Build a **sentence autocomplete system**
* Deploy as a **web app using Streamlit**

---

## 📚 Learning Outcomes

Through this project you will learn:

* NLP text preprocessing
* Tokenization and sequence padding
* RNN architecture
* Next word prediction models
* Deep Learning with TensorFlow/Keras

---

## 👩‍💻 Author

**Ishwarya Kunduru**

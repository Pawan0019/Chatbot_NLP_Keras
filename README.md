# Chatbot Using NLTK & Keras

## Description
A simple, interactive chatbot built using Python, Natural Language Processing (NLTK), and Deep Learning (Keras/TensorFlow). The bot classifies user inputs into predefined "intents" and responds intelligently through a desktop graphical user interface (GUI).

## Features
- Interactive desktop chat interface.
- Natural Language Processing with NLTK for text preprocessing (tokenization, lemmatization).
- Deep Learning model powered by Keras and TensorFlow.
- Easily customizable intent dataset.

## Tech Stack
- **Python 3**
- **NLTK** (Natural Language Toolkit)
- **Keras** & **TensorFlow**
- **Tkinter** (for the GUI)

## How It Works
1. **Data Processing:** The application reads `intents.json`, which contains patterns (user messages) and corresponding responses. It tokenizes and lemmatizes the text to understand the base words.
2. **Model Training:** A neural network (`train_chatbot.py`) is trained on this data to classify which "intent" a user's message belongs to.
3. **Inference:** When you type a message in the GUI (`chatgui.py`), the trained model predicts the intent and randomly picks an appropriate response from `intents.json`.

## How to Run

1. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Train the Model:**
   *(Note: You must run this command whenever you update `intents.json`)*
   ```bash
   python train_chatbot.py
   ```

3. **Start the Chatbot:**
   ```bash
   python chatgui.py
   ```

## Example Input/Output
**User:** Hello!  
**Bot:** Hi! It's great to see you. What's on your mind?  

**User:** Can you tell me a joke?  
**Bot:** Why did the scarecrow win an award? Because he was outstanding in his field!

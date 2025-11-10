# 🤖 ChatGPT Clone using OpenAI + Gradio

A simple ChatGPT-like web app built with **Python**, **Gradio**, and **OpenAI API**, deployable directly in **Google Colab** or locally. This project demonstrates how to create a conversational chatbot with persistent chat history and OpenAI's GPT model.

---

## 🚀 Features

* Interactive chat interface powered by **Gradio**
* Uses **OpenAI GPT-4-turbo** model for responses
* Works directly in **Google Colab** or local Python environment
* Lightweight and beginner-friendly setup



---

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/ChatGPT-Clone.git
cd ChatGPT-Clone
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Add Your OpenAI API Key

Edit the following line in `app.py`:

```python
client = OpenAI(api_key="YOUR_OPENAI_API_KEY")
```

> ⚠️ Never share or upload your real API key publicly.

Alternatively, store it in a `.env` file:

```
OPENAI_API_KEY=your_api_key_here
```

And update the code:

```python
from dotenv import load_dotenv
import os

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
```

---

## ▶️ Run the Application

### In Google Colab:

Simply run all cells in the notebook. Gradio will display a **shareable public link**.

### Locally:

```bash
python app.py
```

Then open the link printed in the terminal.

---

## 📜 Example Output

```
User: Hello, who are you?
AI: I am ChatGPT Clone AI Robot, here to assist you with your questions!
```

---

## 📦 requirements.txt

```
gradio
openai
python-dotenv
```



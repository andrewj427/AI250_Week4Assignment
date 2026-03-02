# Python Code Explainer

A command-line tool that uses a locally running Ollama LLM (llama3) to explain Python code in plain English and add inline comments.

---

## Prerequisites

- Python 3.8+
- [Ollama](https://ollama.com) installed and running

---

## Setup & Run Instructions

### 1. Install Ollama
Download and install Ollama from https://ollama.com

### 2. Pull the llama3 model
```bash
ollama pull llama3
```

### 3. Start Ollama (if not already running)
```bash
ollama serve
```
> You can verify it's running by visiting http://localhost:11434 in your browser.


### 4. Install Python dependencies
```bash
pip install -r requirements.txt
```

### 5. Run the app
```bash
python main.py
```

---

## How to Use

1. Run the app with `python Week4_assignment.py`
2. Paste any Python code into the terminal
3. Shift+Enter, Type `END` and press Enter
4. The app will output:
   - A plain English explanation of what your code does
   - Your code with helpful inline comments added

---

## Troubleshooting

- **"Could not connect to Ollama"** — Make sure `ollama serve` is running in a separate terminal
- **Slow response** — First run may be slow as the model loads into memory; subsequent runs are faster
- **Model not found** — Run `ollama pull llama3` to download the model

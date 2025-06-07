# 🧠 Implementing a Basic RAG Pipeline

## 📦 Libraries and Frameworks Used

- `datasets`
- `huggingface_hub`
- `langchain`
- `langchain_gemini`
- `faiss`
- `streamlit`
---

## 🚀 Project Setup and Execution

The easiest way to run this project is via **Google Colab**.

---

### 🔐 API Keys Required

Before running the notebook, make sure you have the following:

- [🔑 Google Gemini API Key](https://aistudio.google.com/app/apikey?hl=ru)  
- [🔑 Hugging Face API Token](https://huggingface.co/settings/tokens)

---

### 📂 Opening the Notebook in Colab

To open the `rag.ipynb` notebook:

- Navigate to the file and click **"Open with Colab"** at the top,  
  **OR**
- Use [this direct link](https://colab.research.google.com/github/mikolaura/impleting_basic_rag_pipeline/blob/main/rag.ipynb) 
---

### ⚙️ Installing Dependencies

Once the notebook is open:

- Run the **first three cells** to install and load all required libraries.

---

## 🧭 Choose Your Workflow

This notebook supports **three execution paths** depending on your use case.

---

### 1. 🛠️ Build from Scratch

Create a vector store from a dataset:

- Run **all cells** up to the one titled `Alternative: Load vector store`.
- After the command:
  ```python
  !huggingface-cli login
  ```
  input your Hugging Face token when prompted. **Do not** save it as a Git credential.
- After the line:
  ```python
  os.environ['GOOGLE_API_KEY'] = getpass.getpass()
  ```
  input your **Google API key** manually.

---

### 2. 🗃️ Use Prebuilt Vector Store (CLI)

Run the pipeline using a prebuilt vector store via command-line interface:

- Start from the cell titled `Alternative: Load vector store`.
- Stop at the cell titled `OPTIONAL: CREATE WEB-GUI USING STREAMLIT`.
- After:
  ```python
  os.environ['GOOGLE_API_KEY'] = getpass.getpass()
  ```
  input your **Google API key** manually.

---

### 3. 🌐 Use Prebuilt Vector Store (Web UI)

Run the RAG pipeline through a web-based interface:

- Start from the cell titled `OPTIONAL: CREATE WEB-GUI USING STREAMLIT`.
- Continue to the end of the notebook.
- After you run last command open link that was created, but before save ip adress that you get from line `!wget -q -O - https://loca.lt/mytunnelpassword` and paste it into text box
- After you opened streamlit app you need to paste google api key into correspond text box. And after you can anything that correspond to data in dataset
---

## ⚠️ Important Reminder

> ✅ **Make sure to install all required packages before running any of the workflows above!**

---
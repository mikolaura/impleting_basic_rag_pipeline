# 🧠 Implementing a Basic RAG Pipeline

A simple yet functional Retrieval-Augmented Generation (RAG) pipeline using Google Gemini and Hugging Face datasets. Includes three execution paths: from-scratch, CLI-based, and web UI via Streamlit.

---

## 📆 Libraries and Frameworks Used

* [`datasets`](https://huggingface.co/docs/datasets)
* [`huggingface_hub`](https://huggingface.co/docs/huggingface_hub)
* [`langchain`](https://python.langchain.com/)
* [`langchain_gemini`](https://github.com/langchain-ai/langchain)
* [`faiss`](https://github.com/facebookresearch/faiss)
* [`streamlit`](https://streamlit.io/)

---

## 🚀 Project Setup & Execution

This project is best run via **Google Colab**.

---

## 🔐 Required API Keys

Before executing the notebook, ensure you have the following:

* [🔑 Google Gemini API Key](https://aistudio.google.com/app/apikey?hl=ru)
* [🔑 Hugging Face API Token](https://huggingface.co/settings/tokens)

---

## 📂 Open the Notebook in Colab

* Navigate to the file and click **"Open with Colab"**,
  **OR**
* Use this [direct link to `rag.ipynb`](https://colab.research.google.com/github/mikolaura/impleting_basic_rag_pipeline/blob/main/rag.ipynb)

---

## ⚙️ Installing Dependencies

Once the notebook is open, run the **first three cells** to install and import all required libraries.

---

## 🔝 Choose Your Workflow

You can run this notebook in **three different ways**:

### 1. 🛠️ Build from Scratch

Create a new vector store from the dataset:

* Run all cells up to `Alternative: Load vector store`.
* Authenticate with:

  ```bash
  !huggingface-cli login
  ```
* Enter your Hugging Face token (do **not** save as Git credential).
* Enter your Google API Key when prompted:

  ```python
  os.environ['GOOGLE_API_KEY'] = getpass.getpass()
  ```

---

### 2. 🗓️ Use Prebuilt Vector Store (CLI)

Use the pipeline with a prebuilt vector store:

* Start from the cell titled `Alternative: Load vector store`.
* Stop before `OPTIONAL: CREATE WEB-GUI USING STREAMLIT`.
* Provide your Google API Key when prompted.

---

### 3. 🌐 Use Prebuilt Vector Store (Web UI)

Run the RAG pipeline via a simple Streamlit app:

* Start from `OPTIONAL: CREATE WEB-GUI USING STREAMLIT`.
* Run all remaining cells.
* When prompted:

  1. Run the command:

     ```bash
     !wget -q -O - https://loca.lt/mytunnelpassword
     ```
  2. Copy the generated tunnel password.
  3. Paste it into the Colab prompt when asked.
  4. After the Streamlit app opens, paste your Google API Key into the input box.
  5. Ask questions related to the dataset.

---

## ⚠️ Reminder

> ✅ Make sure to install all dependencies **before** executing any of the workflows.

---

## 📚 Dataset Information

You can choose between two dataset sources:

* `text_with_empty_vector.csv` *(Not recommended)*
* ✅ Recommended: [Hugging Face Dataset: `wikipedia_rag`](https://huggingface.co/datasets/uran050311/wikipedia_rag)

---

## 🧠 FAISS Vector Store

This repository includes a folder called `my_faiss_index/` which contains all the files generated when saving the vector store to disk.

---

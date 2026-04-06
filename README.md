# 🤖 Insurance Bot (IndiaFirst Life Assistant)

An AI-powered **Insurance Chatbot** built using **Streamlit, ThirdAI NeuralDB, and OpenAI GPT**, designed to answer user queries based strictly on IndiaFirst Life insurance policy documents.

---

## 🚀 Features

* 📄 **Document-based Q&A** using multiple insurance PDFs
* 🧠 **Semantic Search** powered by ThirdAI NeuralDB
* 🔍 **Query Expansion** using OpenAI for better retrieval
* ⚡ **Fast Response Generation** with GPT model
* 📊 **Accurate Data Extraction** (especially numerical/tabular data)
* 💬 **Interactive Chat UI** using Streamlit
* 🇮🇳 Focused on **Indian insurance policies (INR values)**

---

## 🏗️ Tech Stack

* **Frontend:** Streamlit
* **Backend:** Python
* **AI/ML:**

  * ThirdAI NeuralDB (document retrieval)
  * OpenAI GPT (answer generation)
* **Libraries:**

  * `streamlit`
  * `thirdai`
  * `openai`
  * `nltk`

---

## 📂 Project Structure

```
.
├── app.py (or D.py)
├── Policy/ (PDF documents)
├── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd insurance-bot
```

### 2. Install dependencies

```bash
pip install streamlit thirdai openai nltk
```

### 3. Set Environment Variables

```bash
export THIRD_AI_KEY=your_thirdai_key
export OPEN_AI_KEY=your_openai_key
```

*(Windows users can use `set` instead of `export`)*

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

---

## 📌 How It Works

1. **Document Loading**

   * Insurance PDFs are loaded into ThirdAI NeuralDB

2. **Query Processing**

   * User enters a question
   * Multiple related queries are generated using OpenAI

3. **Search & Retrieval**

   * NeuralDB retrieves relevant document chunks

4. **Ranking**

   * Uses **Reciprocal Rank Fusion (RRF)** to improve relevance

5. **Answer Generation**

   * GPT generates a response based only on retrieved context

---

## 🧠 Key Functionalities

### 🔍 Query Expansion

Generates multiple variations of user queries to improve search accuracy.

### 📚 Context Retrieval

Extracts top relevant document sections.

### 🧮 Data-Focused Answers

* Prioritizes:

  * Numerical values
  * Premiums
  * Age limits
  * Policy benefits

### 📊 Tabular Data Handling

Special attention to extracting structured data from policy documents.

---

## 💡 Example Queries

* What is the minimum age for this policy?
* What is the premium amount?
* What are the maturity benefits?
* What is the maximum entry age?

---

## ⚠️ Important Notes

* Answers are **strictly based on provided documents**
* No external knowledge is used
* Designed specifically for **IndiaFirst Life policies**
* Handles edge cases like:

  * Entry age vs maturity age
  * Different policy options (Definite vs Whole Life)

---

## 🔒 Limitations

* Depends on document quality and formatting
* Requires API keys for ThirdAI and OpenAI
* Not suitable for real-time policy updates without reloading documents

---

## 📈 Future Improvements

* Upload documents dynamically via UI
* Add multi-language support
* Improve UI/UX design
* Add voice input/output
* Fine-tuned domain-specific LLM

---

## 👩‍💻 Author

Developed as an AI-powered document assistant for insurance domain use cases.

---

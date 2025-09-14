# 📧 Cold Email Generator using GenAI

This project automates **cold email generation for business outreach**.  
It extracts job requirements from company websites, matches them with your **skills & projects** (stored in a vector database), and then generates a **personalized cold email** using **LangChain + Groq LLMs**.

---

## 📌 Features

- 🔍 Extract job postings from company websites (via **Selenium**)  
- 📊 Store & query portfolio data in **ChromaDB (Vector Database)**  
- 🧠 Generate emails using **LangChain chains** with **Groq LLM** backend  
- 🎨 Interactive UI powered by **Streamlit**  
- ⚡ Custom portfolio integration (`my_portfolio.csv`) for personalized skills/projects  

---

## 🛠️ Tech Stack

- **LangChain** (`langchain`, `langchain-community`, `langchain-groq`)  
- **Groq LLM API** for text generation  
- **Unstructured** (document parsing)  
- **Selenium** (job posting extraction)  
- **ChromaDB** (vector store for portfolio & skills)  
- **Streamlit** (UI)  
- **Pandas** (data handling)  
- **dotenv** (manage API keys & config)  



## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/sarthakpande108/Cold-Email-using-GenAI.git
cd Cold-Email-using-GenAI



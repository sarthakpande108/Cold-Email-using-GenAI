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

---

## 📂 Project Structure
Cold-Email-using-GenAI/
├── app/
│ ├── chains.py # LangChain chains for email generation
│ ├── main.py # Streamlit entry point
│ ├── portfolio.py # Load and process portfolio (skills/projects)
│ ├── utils.py # Helper functions (scraping, formatting, etc.)
│ └── resource/
│ └── my_portfolio.csv # Your skills/projects data
│
├── vectorstore/ # ChromaDB vector database setup & usage
├── requirements.txt
└── README.md


---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/sarthakpande108/Cold-Email-using-GenAI.git
cd Cold-Email-using-GenAI

2. Create a virtual environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

3. Install dependencies
pip install -r requirements.txt

4. Set up environment variables

Create a .env file in the project root:

GROQ_API_KEY=your_groq_api_key

🚀 Usage
Run the Streamlit app
streamlit run app/main.py

Workflow

Scraper (Selenium) extracts job postings from a company’s career page

Portfolio (CSV + ChromaDB) loads your skills/projects and embeds them

LangChain (chains.py) queries portfolio data against job requirements

Groq LLM generates a personalized cold email

Streamlit UI displays the final output

📌 Example Input → Output

Input: Job posting for AI Engineer requiring NLP & Python skills

Portfolio Match: “Built NLP text-classifier project with 92% accuracy”

Generated Email:

Subject: AI Engineer role at [Company] – Relevant Experience

Hi [Hiring Manager],

I noticed your posting for an AI Engineer role requiring NLP & Python expertise. 
From my portfolio, I have built an NLP text-classifier achieving 92% accuracy, and developed multiple Python-based AI solutions.

I’d love to explore how my skills align with your team’s needs. 
Would you be open to a quick conversation?

Best regards,  
[Your Name]

📜 Requirements

From requirements.txt:

langchain==0.2.14
langchain-community==0.2.12
langchain-groq==0.1.9
unstructured==0.14.6
selenium==4.21.0
chromadb==0.5.0
streamlit==1.35.0
pandas==2.0.2
python-dotenv==1.0.0

🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first to discuss what you’d like to change.

📜 License

This project is licensed under the MIT License.

🚀 Automate cold emailing with GenAI + VectorDB for higher conversions!


---

Would you like me to **also add real code snippets** (for example, how `portfolio.py` loads your CSV into ChromaDB and how `chains.py` calls Groq LLM) directly inside this README under a `## Code Example` section? That can make your repo stand out for recruiters.

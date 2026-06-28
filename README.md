Cold Email Generator

Overview:
The Cold Email Generator is a Generative AI‑powered application that automatically creates professional job application emails based on job postings.
It uses LangChain, Groq’s Llama 3.3 model, and Streamlit to extract job details from career pages and generate personalized cold emails for Computer Science‑related roles.

Features:

1.Scrapes job descriptions directly from career websites.Extracts structured data (role, experience, skills, 2.description) using Groq LLM.
3.Matches relevant portfolio links via ChromaDB vector search.
4.Generates polished, professional cold emails automatically.
5.Interactive Streamlit UI with real‑time generation and error handling.


⚙️ Tech Stack

Component	               Purpose
Python 3.13	               Core language
Streamlit                  Front‑end interface
LangChain + Groq API	   LLM integration
ChromaDB	               Portfolio vector storage
pandas	                   CSV data handling
dotenv	                   Secure API‑key management


Cold email generator/
│
├── app/
│   ├── resource/
│   │   ├── .env
│   │   ├── my_portfolio.csv
│   ├── chains.py
│   ├── main.py
│   ├── portfolio.py
│   ├── utils.py
│   ├── requirement.txt
│
├── vectorstore/
│   ├── chroma.sqlite3
│
├── README.md


Future Improvements:

Add tone/style selector (Formal, Friendly, Confident).
Enable multiple job URLs at once.
Integrate resume upload and automatic attachment.
Deploy on Streamlit Cloud or Azure.

Author
Aditi Phulre  

Cold Email Generator – Powered by LangChain & Groq LLM
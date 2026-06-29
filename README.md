# __Cold Email Generator__

## __Overview__
The **Cold Email Generator** is a Generative AI‑powered application that automatically creates professional job application emails based on job postings.  

It uses **LangChain**, **Groq’s Llama 3.3 model**, and **Streamlit** to extract job details from career pages and generate personalized cold emails for Computer Science‑related roles.

---

## __Features__
- Scrapes job descriptions directly from career websites  
- Extracts structured data (role, experience, skills, description) using Groq LLM  
- Matches relevant portfolio links via ChromaDB vector search  
- Generates polished, professional cold emails automatically  
- Interactive Streamlit UI with real‑time generation and error handling  

---

## __Tech Stack__
- **Python 3.13** → Core language  
- **Streamlit** → Front‑end interface  
- **LangChain + Groq API** → LLM integration  
- **ChromaDB** → Portfolio vector storage  
- **pandas** → CSV data handling  
- **dotenv** → Secure API‑key management  

---

## __Groq’s Llama 3.3 Model Usage__
The LLM is the intelligence layer in my project. It does two main things:  

1. **Understanding job postings**  
   - Scraped text from a careers page is passed into Groq LLM  
   - Using prompt instructions, the model identifies key details (role, experience, skills, description)  
   - Outputs structured JSON format for easy processing  

2. **Generating cold emails**  
   - Structured job data + portfolio links are fed into Groq LLM with a second prompt  
   - Composes a professional, tailored email highlighting background and skills  
   - Output is plain text, displayed in Streamlit  

---

## __Block Diagram__
![Block Diagram](imgs/block_diagram.png)

---

## __File Structure__
![File Structure](imgs/File_struct.png)

---

## __Workflow__
- User Input → Paste job posting URL  
- Scraping & Cleaning → Extract and preprocess text  
- Job Extraction → Groq LLM converts text into structured JSON  
- Portfolio Matching → ChromaDB finds relevant links  
- Email Generation → Groq LLM writes professional cold email  
- Display → Streamlit shows the final email  

---

## __Generated Email Example__
![Generated Email Example](imgs/generated_email.png)

---

## __Future Improvements__
- Add tone/style selector (Formal, Friendly, Confident)  
- Enable multiple job URLs at once  
- Integrate resume upload and automatic attachment  
- Deploy on Streamlit Cloud or Azure  

---

## __Author__
**Aditi Phulre**  
Cold Email Generator – Powered by LangChain & Groq LLM  

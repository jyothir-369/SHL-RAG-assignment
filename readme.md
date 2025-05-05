🧠 SHL Generative AI Product Recommender
This project is a smart product recommendation system developed as part of the SHL AI Intern assignment. It leverages a Retrieval-Augmented Generation (RAG) pipeline combined with an LLM-based reranking mechanism to recommend SHL assessments based on natural language job descriptions or queries.

🚀 Key Features
🔍 Semantic search over SHL’s assessment catalog using FAISS

🧠 Reranking powered by Claude 3 Haiku for improved result accuracy

📋 Displays metadata: duration, test type, remote compatibility, adaptive support, and download availability

🎯 Precision Mode: Retrieves the top 3 most relevant assessments

⚙️ FastAPI backend with /recommend endpoint

🖼️ Streamlit frontend for easy interaction

💬 Bonus: Conversational RAG chatbot (step1_rag.py) using Gemini, DeepSeek, or LLaMA3

📁 Project Structure
bash
Copy
Edit
shl-recommender/
├── data/                      # Product metadata and FAISS index
├── recommender/              # Core recommendation logic
│   └── core.py
├── streamlit_app/            # Streamlit-based frontend
│   └── app.py
├── api/                      # FastAPI backend server
│   └── main.py
├── step1_rag.py              # Optional multimodal chatbot
├── SHL_Generative_AI_Summary.pdf  # Summary report
├── requirements.txt          # Python dependencies
├── README.md                 # Project documentation
🧰 Tech Stack
Component	Tool/Library
Embeddings	BAAI bge-small-en-v1.5
Vector DB	FAISS
Reranker LLM	Claude 3 Haiku (via OpenRouter)
Frontend	Streamlit
Backend	FastAPI
Chatbot Models	Gemini, DeepSeek, LLaMA
Scraping	Selenium + BeautifulSoup

▶️ Getting Started
1. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
2. Launch the FastAPI Backend
bash
Copy
Edit
uvicorn api.main:app --reload
Test endpoint:
http://localhost:8000/recommend?q=productivity manager

3. Start the Streamlit UI
bash
Copy
Edit
streamlit run streamlit_app/app.py
Access frontend:

Local: http://localhost:8501

Network: http://192.168.1.16:8501

🌐 Deployment
Component	URL
Live UI	https://ragassess-shl.streamlit.app/
API Endpoint	Coming soon
GitHub Repo	SHL-RAG-assignment

✅ Project Deliverables
✅ Top 3 SHL product recommendations per query

✅ Fully functional API and frontend

✅ Complete metadata presentation

✅ Optional: Chatbot variant with multimodal support

✅ Final summary document: SHL_Generative_AI_Summary.pdf

📬 Contact
For any questions, suggestions, or feedback — feel free to reach out via my portfolio:
👉 https://jyothir-369.github.io/BJR/

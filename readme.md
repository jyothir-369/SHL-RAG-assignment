🧠 SHL Generative AI Product Recommender
A smart product recommendation system developed as part of the SHL AI Intern assignment. It uses a Retrieval-Augmented Generation (RAG) pipeline and an LLM-based reranking mechanism to recommend SHL assessments based on natural language job descriptions or queries.

🚀 Key Features
🔍 Semantic Search: Over SHL’s assessment catalog using FAISS

🧠 Reranking: Powered by Claude 3 Haiku for higher accuracy

📋 Comprehensive Display: Shows duration, test type, remote compatibility, adaptive support, and download availability

🎯 Precision Mode: Retrieves the top 3 most relevant assessments

⚙️ FastAPI Backend: /recommend endpoint for integration

🖼️ Streamlit Frontend: Clean, interactive UI

💬 Bonus: Conversational RAG chatbot (via step1_rag.py) using Gemini, DeepSeek, or LLaMA3

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
Vector Database	FAISS
Reranker LLM	Claude 3 Haiku (via OpenRouter)
Frontend	Streamlit
Backend	FastAPI
Chatbot Models	Gemini, DeepSeek, LLaMA
Web Scraping	Selenium + BeautifulSoup

▶️ Getting Started
Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
Launch the FastAPI Backend

bash
Copy
Edit
uvicorn api.main:app --reload
Test endpoint: http://localhost:8000/recommend?q=productivity manager

Start the Streamlit UI

bash
Copy
Edit
streamlit run streamlit_app/app.py
Access locally: http://localhost:8501

On network: http://192.168.1.16:8501

🌐 Deployment
Component	URL
Live UI	ragassess-shl.streamlit.app
API Endpoint	Coming soon
GitHub Repo	SHL-RAG-assignment

✅ Project Deliverables
✅ Top 3 SHL product recommendations per query

✅ Fully functional API and frontend

✅ Complete metadata display

✅ Optional: Multimodal chatbot with LLM integration

✅ Final summary document: SHL_Generative_AI_Summary.pdf

📬 Contact
For questions, suggestions, or feedback, feel free to reach out via my portfolio.

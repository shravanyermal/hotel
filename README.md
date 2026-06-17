HotelGPT – Intelligent Hotel Reception Assistant
Overview

HotelGPT is an intelligent hotel reception chatbot powered by Retrieval-Augmented Generation (RAG) and Large Language Models (LLMs). The chatbot provides instant and accurate responses to guest queries by retrieving information from hotel documents, FAQs, policies, amenities, and service information.

The system combines semantic search using FAISS vector databases with Generative AI to deliver context-aware answers, enhancing the guest experience and reducing the workload of hotel staff.

Features
Natural language hotel query answering
Retrieval-Augmented Generation (RAG)
Semantic search using FAISS
Conversational AI interface
Hotel policy and FAQ assistance
Amenities and services information
Context-aware responses
Streamlit web interface
Fast document retrieval
Scalable knowledge base
Technology Stack
Frontend
Streamlit
Backend
Python
AI & Machine Learning
LangChain
Sentence Transformers
FAISS Vector Database
Groq LLM / OpenAI-compatible APIs
Document Processing
PyPDF
Recursive Character Text Splitter
Project Architecture
Hotel documents are uploaded and processed.
Documents are split into smaller chunks.
Text embeddings are generated using Sentence Transformers.
Embeddings are stored in a FAISS vector database.
User queries are converted into embeddings.
Relevant document chunks are retrieved.
Retrieved context is passed to the LLM.
The chatbot generates accurate responses based on retrieved information.
Installation
Clone Repository
git clone https://github.com/yourusername/hotel-reception-chatbot-rag.git
cd hotel-reception-chatbot-rag
Install Dependencies
pip install -r requirements.txt
Required Packages
streamlit
langchain
langchain-community
langchain-openai
langchain-huggingface
langchain-text-splitters
sentence-transformers
faiss-cpu
pypdf
openai
Project Structure
hotel-reception-chatbot-rag/
│
├── app.py
├── requirements.txt
├── README.md
├── faiss_db/
│   ├── index.faiss
│   └── index.pkl
└── hotel_data/
Configuration

Add your API key in Streamlit Secrets:

GROQ_API_KEY="your_api_key_here"
Running the Application
streamlit run app.py

The application will be available at:

http://localhost:8501
Deployment

The application can be deployed using Streamlit Community Cloud.

Push the project to GitHub.
Connect the repository to Streamlit Cloud.
Configure API secrets.
Deploy the application.
Sample Questions
What are the hotel check-in and check-out timings?
Does the hotel provide airport pickup?
What amenities are available for guests?
Is Wi-Fi available throughout the hotel?
What is the cancellation policy?
Does the hotel have a swimming pool or gym?
Are pets allowed in the hotel?
Future Enhancements
Voice-enabled interaction
Multi-language support
Reservation and booking integration
Sentiment analysis
Personalized guest recommendations
Integration with hotel management systems

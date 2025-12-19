🩺 MediConsult AI: Medical Chatbot
MediConsult AI is a state-of-the-art medical assistant designed to provide instant health information using a Retrieval-Augmented Generation (RAG) pipeline. It combines a clean, professional "MediConsult" dashboard UI with powerful AI models.

🚀 Features
Professional Dashboard UI: A clean, responsive sidebar-based layout optimized for medical consultations.

Knowledge Base Shortcuts: Quick-access buttons for common health topics like heart health, stress management, and sleep hygiene.

RAG Architecture: Uses Pinecone as a vector database to retrieve context from specialized medical documents.

Intelligent Responses: Powered by Llama 3.1 via Groq for high-speed, accurate medical explanations.

Markdown Support: Bot responses are beautifully formatted with bold text, bullet points, and headers for better readability.

🛠️ Technology Stack
Frontend: HTML5, CSS3 (Inter Font, Font Awesome), JavaScript (Marked.js).

Backend: Flask (Python).

AI Framework: LangChain.

Vector Database: Pinecone.

LLM Model: Llama-3.1-8b-instant (via Groq API).

Embeddings: HuggingFace Sentence-Transformers.

📂 Project Structure
Plaintext

Medical-Chatbot/
│
├── static/              # CSS and images (logo.png)
├── templates/           # HTML files (chat.html)
├── src/                 # Helper functions and prompt templates
├── app.py               # Main Flask application
├── requirements.txt     # Python dependencies
├── .env                 # API Keys (Not uploaded to GitHub)
└── data/                # Source medical PDFs

⚙️ Installation & Setup
1. Clone the Repository
Bash

git clone https://github.com/your-username/medical-chatbot.git
cd medical-chatbot
2. Set Up Environment
It is recommended to use a virtual environment:

Bash

conda create -n medibot_new python=3.10
conda activate medibot_new
pip install -r requirements.txt
3. Configure API Keys
Create a .env file in the root directory and add your keys:

Plaintext

PINECONE_API_KEY = "your_pinecone_key"
GROQ_API_KEY = "your_groq_key"
4. Run the Application
Bash

python app.py
Visit http://localhost:8080 in your browser.

📄 Requirements
The project depends on the following libraries:

langchain

langchain_groq

pinecone-client

flask

sentence-transformers

pypdf

🛡️ Disclaimer
This chatbot is for informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.
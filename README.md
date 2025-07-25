# Azure-Cloud-Deployment

# 💬 ChatWithPDF Project Using Groq-LLAMA Model

This project allows users to **interact with PDF documents** using **RAG (Retrieval-Augmented Generation)** and **LLaMA models** via **Groq API**. Built using LangChain, it supports intelligent question-answering from uploaded documents.

---

## 📁 Project Structure

```plaintext
ChatWithPDF-Project Using Groq-llama model/
├── app.py                  # Main Streamlit app
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (e.g., GROQ_API_KEY)
├── utils/                  # Modular utility code
│   ├── document_loader.py     # Loads and parses PDF files
│   ├── vectorstore_setup.py   # Chunks, embeds, and stores documents in a FAISS vectorstore
│   └── chain_factory.py       # Builds Conversational Retrieval Chain using ChatGroq


## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/chatwithpdf-groq-llama.git
cd chatwithpdf-groq-llama

2. Create a virtual environment (recommended)

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies
pip install -r requirements.txt

4. Add your Groq API key to .env

GROQ_API_KEY=your_actual_groq_api_key
🔒 Note: Never commit .env to version control.

🧠 Model Used
This app uses the Groq API with the LLaMA 3.3 70B Versatile model to answer questions based on content retrieved from uploaded PDFs.

☁️ Deployment to Azure
You can deploy this Streamlit app to Azure Web App using the following steps:

1. Prepare Azure App Service
Create a new App Service instance

Choose Python runtime (3.10 or above)

Enable deployment from GitHub or local ZIP file

2. Set environment variables in Azure
Go to your App Service > Configuration > Application settings:

Add key: GROQ_API_KEY

Value: your_groq_api_key

3. Deploy your code
Push your code to Azure using your preferred CI/CD method.

🖥️ Running Locally

streamlit run app.py
🧾 Features
📄 Upload and process multiple PDF files

🧠 Uses LLaMA 3.3 70B via Groq for high-performance responses

📚 Retrieves document chunks using FAISS vector store

💬 Conversational interface with memory

⚡ RAG-powered Q&A system

🧠 Future Enhancements
Add support for DOCX, TXT files

Integrate Google or Azure Vision APIs for scanned PDFs

Save and reload chat sessions

UI theming and personalization

📄 License
MIT License © 2025

👨‍💻 Author
Built with ❤️ by Ajeetkumar



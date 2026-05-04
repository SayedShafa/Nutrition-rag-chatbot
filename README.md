
**RAG Chatbot on Bangladesh National Dietary Guidelines**
A **Retrieval-Augmented Generation (RAG)** based chatbot that answers questions  about **food, nutrition, and health** based on the official "National Dietary Guidelines for Bangladesh" PDF. Built with **LangChain**, **FAISS**, **Ollama (Local LLM)**. Fully offline, no API keys required.
Just ask a question in plain English or Bengali — and it will give you an answer instantly!

**Features**
- **PDF Text Extraction** – Loads and processes PDF documents
- **Chunking & Embedding** – Splits text into chunks and converts to vector embeddings  
- **FAISS Vector Database** – Stores embeddings for fast similarity search  
- **Local LLM (Ollama)** – Uses `llama3.2:1b` (free, offline, no API key)  
- **RAG Pipeline** – Retrieves relevant chunks and generates accurate answers  
- **Interactive Chat** – Ask questions in real-time, exit with `exit`  
- **Source Tracking** – Shows which PDF sections were used to generate the answer

**Tech Stack**
- Python 3.10
- LangChain
- FAISS (Vector Database)
- HuggingFace Embeddings (all-MiniLM-L6-v2)
- Ollama (llama3.2:1b)
- PyPDFLoader / pypdf

**Libraries Used**

- PyPDFLoader (langchain-community)
- RecursiveCharacterTextSplitter (langchain-text-splitters)
- HuggingFaceEmbeddings (langchain-huggingface)
- FAISS (langchain-community)
- ChatOllama (langchain-ollama)
- RetrievalQA (langchain-classic)

**Sample Questions**
- 1.What are the dietary guidelines for diabetes patients?
- 2.How much water should an adult drink daily?
- 3.What foods are recommended for pregnant women?
- 4.What foods are recommended for children aged 2-5 years?
- 5.How much fish and meat is recommended per day?

**Output Example**
- Your Question:  How much water should an adult drink daily according to the guidelines?
- 🌸🌸🌸 Answer: According to the guidelines, an adult should drink at least 10 to 12 glasses of fluid per day. However, it's not explicitly stated how many ounces or milliliters this equates to.

**Purpose:**
- Ask anything about food, diabetes, pregnancy diet, or nutrition
- Get answers directly from the government PDF
- Works fully offline (no internet needed)
- Free — no OpenAI or API costs
- Private — your data stays on your computer

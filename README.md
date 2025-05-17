# 🩺 Medical Advice Chatbot - GenAI 

> An end-to-end AI chatbot for answering medical queries using LLaMA 2, LangChain, Pinecone, and Flask.

---

## 📝 Description  

This project builds a powerful medical chatbot using Meta's LLaMA 2 model. It integrates LangChain for natural language understanding, Pinecone for semantic vector storage, and Flask as the web framework.  

Key features include:  
- Answering medical-related queries with context  
- Local inference using quantized LLaMA 2    
- Flask-based minimal frontend  
- Easy setup with Conda and environment variables  

---

## ✅ Prerequisites  

Make sure you have the following installed before proceeding:  
- [Git](https://git-scm.com/downloads)  
- [Miniconda/Anaconda](https://docs.conda.io/en/latest/miniconda.html)  
- Python 3.8  

---

## 🚀 Installation  

### Step 1: Clone the Repository  
```bash
git clone https://github.com/your-username/medical-chatbot-llama2.git
cd medical-chatbot-llama2
```

### Step 2: Create & Activate Conda Environment  
```bash
conda create -n mchatbot python=3.8 -y
conda activate mchatbot
```

### Step 3: Install Dependencies  
```bash
pip install -r requirements.txt
```

---

## 🔐 Configuration  

### Step 4: Set Up Environment Variables  
Create a `.env` file in the root directory with the following contents:
```env
PINECONE_API_KEY=your_pinecone_api_key
OPENAI_API_KEY = your api key

```

---

## 📥 Model Setup  

### Step 5: Download LLaMA 2 Quantized Model  

Go to the [Hugging Face repo](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main) and download:

```
llama-2-7b-chat.ggmlv3.q4_0.bin
```

Place it inside the `model/` directory.

---

## ⚙️ Run the Project  

### Step 6: Generate the Vector Index  
```bash
python store_index.py
```

### Step 7: Start the Chatbot App  
```bash
python app.py
```

Visit `http://localhost:5000` in your browser.

---

## 🧰 Tech Stack  

- 🐍 Python 3.8  
- 🌐 Flask  
- 🧠 LangChain  
- 🌲 Pinecone  
- 🤖 Meta LLaMA 2 (GGML)  
- 📦 Conda  

---

## 📂 Folder Structure  

```bash
medical-chatbot/
│
├── app.py                 # Main Flask app
├── store_index.py         # Script to store vector index in Pinecone
├── model/                 # Folder to store downloaded LLaMA model
├── templates/             # HTML templates
├── static/                # CSS/JS/assets
├── requirements.txt
├── .env
└── README.md
```

---

## 🧑‍💻 Author  

- **N. Harintharan**  
- GitHub: [@Harintharan](https://github.com/Harintharan)  
- Email: nharintharan@gmail.com  

---

## 📄 License  

This project is licensed under the **MIT License**. See [LICENSE](./LICENSE) for more details.
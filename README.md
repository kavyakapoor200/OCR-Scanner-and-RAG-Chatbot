
### 📌 **README for Colab-Based RAG Chatbot & OCR System**  
```markdown
# 🚀 AI Engineer Internship Projects (Google Colab)

This repository contains two AI projects built as part of my AI Engineer Internship assignment:  

1️⃣ **RAG Chatbot** – A Retrieval-Augmented Generation (RAG) chatbot that allows users to upload documents (PDF, DOCX, TXT) and ask questions about them.  
2️⃣ **OCR System** – A text extraction tool using **Tesseract OCR** to extract text from images and scanned documents.

Both projects were developed in **Google Colab** and can be executed directly from there. 🚀  

---

## 📌 **Project 1: RAG Chatbot** (Retrieval-Augmented Generation)

### ✨ **Features**
- 📄 Upload multiple documents (PDF, DOCX, TXT)
- 🔍 Perform **semantic search** over the documents using **ChromaDB**
- 🤖 Ask questions, and get AI-generated answers based on document context
- 🎤 Uses **Mistral-7B / GPT-3.5-turbo** for response generation
- 🌐 **Hosted via ngrok** for external access

### 🛠 **Tech Stack**
- **Google Colab** (Execution)
- **Streamlit** (UI Framework)
- **LangChain** (RAG Framework)
- **ChromaDB** (Vector Storage)
- **Mistral-7B / GPT-3.5-turbo** (AI Model)
- **PyPDFLoader, Docx2txtLoader, TextLoader** (Document Parsing)
- **ngrok** (To expose Colab app to the internet)

### 🚀 **Run in Google Colab**
1. **Open the Colab Notebook**  
   👉 [Colab Link](https://colab.research.google.com/drive/YOUR_NOTEBOOK_ID)  

2. **Install Dependencies**
   ```python
   !pip install streamlit langchain_community chromadb tiktoken pypdf pyngrok
   ```

3. **Run Streamlit in Colab**
   ```python
   !streamlit run app.py & npx localtunnel --port 8501
   ```

4. **Expose the App via ngrok**
   ```python
   !pip install pyngrok
   !ngrok authtoken YOUR_NGROK_AUTH_TOKEN
   !ngrok http 8501
   ```
📌 **Now copy the public URL and access the chatbot!** 🎉  

---

## 📌 **Project 2: OCR System** (Optical Character Recognition)

### ✨ **Features**
- 📷 Extracts text from **images (JPG, PNG) and scanned PDFs**
- 🔍 Uses **Tesseract OCR** for high-accuracy text extraction
- 📥 Supports **batch processing** of multiple files

### 🛠 **Tech Stack**
- **Google Colab** (Execution)
- **Pytesseract** (OCR Engine)
- **OpenCV** (Image Preprocessing)
- **Pandas** (For text processing & storage)

### 🚀 **Run in Google Colab**
1. **Open the Colab Notebook**  
   👉 [Colab Link](https://colab.research.google.com/drive/YOUR_NOTEBOOK_ID)  

2. **Install Dependencies**
   ```python
   !pip install pytesseract opencv-python pandas
   ```

3. **Run the OCR Script**
   ```python
   import pytesseract
   import cv2

   image_path = "sample_image.jpg"  # Replace with uploaded image path
   image = cv2.imread(image_path)
   extracted_text = pytesseract.image_to_string(image)

   print("📝 Extracted Text:\n", extracted_text)
   ```
📌 **This will extract text from the uploaded image!**  

---

## 📌 **Deployment**
### 🌐 **For RAG Chatbot**
1. **Deploy via Colab + ngrok**
2. **Or host on Streamlit Cloud / Hugging Face Spaces**

### ☁️ **For OCR**
- Can be deployed as a **Flask API** in Colab.

---

## 📌 **Project Structure (Colab)**
```bash
📂 AI-Internship-Projects
│── 📂 RAG-Chatbot (Colab Notebook)
│   ├── app.py                # Streamlit RAG Chatbot
│   ├── Colab Notebook        # RAG Chatbot in Google Colab
│
│── 📂 OCR-System (Colab Notebook)
│   ├── ocr_script.py         # OCR Processing Script
│   ├── Colab Notebook        # OCR in Google Colab
│
└── README.md                 # Project Documentation
```

---

## 📌 **Contributing**
Feel free to contribute by creating a pull request! If you find issues, report them in the Issues section.

---

## 📌 **Contact**
🔗 **GitHub:** [github.com/kavyakapoor200](https://github.com/kavyakapoor200)  
📧 **Email:**kavyakapoor869@gmail.com** 
```

---

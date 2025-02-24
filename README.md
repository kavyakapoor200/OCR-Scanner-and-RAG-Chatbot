

### **📌 README.md**  

```markdown
# 🚀 AI Engineer Internship Projects (Google Colab)

This repository contains two AI projects built as part of my AI Engineer Internship assignment:  

1️⃣ **RAG Chatbot** – A Retrieval-Augmented Generation (RAG) chatbot that allows users to upload documents (PDF, DOCX, TXT) and ask questions about them.  
2️⃣ **OCR System** – A text extraction tool using **Tesseract OCR** to extract text from images and scanned documents.

---

## 📂 Project Files

📜 **RAG_chatbot.ipynb** – Google Colab notebook for the Retrieval-Augmented Generation chatbot.  
📜 **OCR.ipynb** – Google Colab notebook for Optical Character Recognition using Tesseract OCR.  
📜 **README.md** – Project documentation.  

---

## 🔹 **Project 1: RAG Chatbot**
### ✨ Features
✔️ Upload and process **PDF, DOCX, and TXT files**  
✔️ Perform **semantic search** using **ChromaDB**  
✔️ **AI-generated answers** using **Mistral-7B / GPT-3.5-turbo**  
✔️ **Streamlit UI** for an interactive chat experience  
✔️ **ngrok integration** for external access  

### 🛠 Tech Stack
- **Streamlit** (Frontend)
- **LangChain** (RAG Framework)
- **ChromaDB** (Vector Storage)
- **Mistral-7B / GPT-3.5-turbo** (AI Model)
- **PyPDFLoader, Docx2txtLoader, TextLoader** (Document Parsing)
- **ngrok** (For public access in Colab)

### 🚀 Run in Google Colab
1. Open the Colab Notebook:  
   👉 [Colab Link]([https://colab.research.google.com/drive/YOUR_NOTEBOOK_ID](https://colab.research.google.com/drive/1Efqak4qS6_Vzws35YI4BwuEbVOUXKJIs?usp=sharing))  
2. Install Dependencies:  
   ```python
   !pip install streamlit langchain_community chromadb tiktoken pypdf pyngrok
   ```
3. Run Streamlit App:  
   ```python
   !streamlit run app.py & npx localtunnel --port 8501
   ```
4. Expose the App via ngrok:  
   ```python
   !pip install pyngrok
   !ngrok authtoken YOUR_NGROK_AUTH_TOKEN
   !ngrok http 8501
   ```
📌 **Now copy the public URL and access the chatbot!** 🎉  

---

## 🔹 **Project 2: OCR System**
### ✨ Features
✔️ Extracts text from **images (JPG, PNG) and scanned PDFs**  
✔️ Uses **Tesseract OCR** for accurate text recognition  
✔️ Supports **batch processing** of multiple files  
✔️ Converts scanned text into **editable formats**  

### 🛠 Tech Stack
- **Google Colab** (Execution)
- **Pytesseract** (OCR Engine)
- **OpenCV** (Image Preprocessing)
- **Pandas** (For text processing & storage)

### 🚀 Run in Google Colab
1. Open the Colab Notebook:  
   👉 [Colab Link]([https://colab.research.google.com/drive/YOUR_NOTEBOOK_ID](https://colab.research.google.com/drive/1vYeEGJaFgrCHAQfK5ER50J4NG5Z1F7-M?usp=sharing))  
2. Install Dependencies:  
   ```python
   !pip install pytesseract opencv-python pandas
   ```
3. Run the OCR Script:  
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

## 🌐 Deployment
### 🔹 **For RAG Chatbot**
- ✅ Deployed via **Colab + ngrok**
- ✅ Can also be hosted on **Streamlit Cloud / Hugging Face Spaces**

### 🔹 **For OCR**
- ✅ Can be deployed as a **Flask API** in Colab

---

## 📌 **Contributing**
💡 If you have suggestions or improvements, feel free to **open an issue** or **submit a pull request**!  

---

## 📌 **Contact**
🔗 **GitHub:** [github.com/kavyakapoor200](https://github.com/kavyakapoor200)  
📧 **Email:** kavyakapoor869@gmail.com
```

---

# Document Translator with Azure Translator API

This project is a **Word document (.docx) translator** built with **Microsoft Azure Translator Text API**, developed in **Python** and designed to run in environments such as **Google Colab**.

The script reads a `.docx` file, translates its content paragraph by paragraph, and generates a new translated document.

---

## 🚀 Technologies used

- Python  
- Azure Translator Text API  
- Requests  
- python-docx  
- Google Colab  

---

## ▶️ How it works

The application performs the following steps:

1. Reads a `.docx` document  
2. Iterates through each paragraph  
3. Sends the text to Azure Translator API  
4. Receives the translated text  
5. Creates a new `.docx` file with the translated content  

---

## ⚙️ Environment configuration

Before running the code, you must configure your **Azure Translator credentials**.

### 🔐 Required variables

```python
subscription_key = "YOUR_AZURE_TRANSLATOR_KEY"
endpoint = "https://api.cognitive.microsofttranslator.com"
location = "eastus2"
language = "pt-br"
```

---

## ▶️ How to run

- Upload your .docx file to the environment
- Update the input file path:
```python
input_file = "/content/music.docx"
```
- Run the script:
```python
translate_document(input_file)
```
- The translated file will be saved with a language suffix:
```python
music_pt-br.docx
```

- Code example:
```python
translate_document("/content/music.docx")
```

- Output:

Original file: music.docx

Translated file: music_pt-br.docx

Each paragraph is translated individually and preserved in the final document.

---

## 🔍 Notes and best practices
- The source language is set to English (from: 'en')
- The target language can be changed using the language variable
- Empty paragraphs are still processed
- Large documents may consume more API quota





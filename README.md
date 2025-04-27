# 📝 Document Summarization and Review Agent using LangGraph

This project is a **document summarization chatbot** built with **LangChain**, **LangGraph**, **Groq**, and **Huggingface embeddings**, running in **Google Colab**. 

It can generate concise summaries from documents, take **user feedback**, and **refine** summaries through multiple review iterations.

---

## 🚀 Features

- 📚 Load and process PDF documents
- 🧠 Summarize documents in **under 50 words**
- 🔄 Review and critique summaries for **accuracy and completeness**
- 🔁 Incorporate **user feedback** to improve summaries
- 🛠️ Built using **StateGraph** and **MemorySaver** from LangGraph
- 🦙 Uses **Groq's LLaMA 3 70B** model for summarization and reviewing
- 🧩 Embeddings generated with **BAAI bge-large-en-v1.5**
- 🖼️ Visualizes the agent flow using **Mermaid Diagrams**

---

## 📂 Project Structure

```bash
📁 document-summarizer-agent/
├── langgraph_summarizer_agent.ipynb             # Main Google Colab notebook
├── EcoSprint_Specification_Document.pdf  # Sample input document
└── README.md                          # Project readme
└── LICENSE.txt                        # LICENSE
```

## 🛠️ Setup Instructions
### 1. Clone the repository:
  ```bash
  git clone https://github.com/shaadclt/LangGraph-Summarizer-Agent.git
  cd LangGraph-Summarizer-Agent
  ```

### 2. Install Dependencies:
In your Google Colab or local environment:
  ```bash
  pip install langchain langgraph langchain_groq langchain_community
  pip install pypdf
  ```

### 3. Set API Keys:
Make sure your Groq API Key is securely available.
In Google Colab:

  ```python
  from google.colab import userdata
  import os
  os.environ["GROQ_API_KEY"] = userdata.get("GROQ_API_KEY")
  ```
### 4. Run the Notebook:
Upload a PDF document (example: EcoSprint_Specification_Document.pdf)

### 5. Execute the notebook step-by-step

## 📜 How It Works
### Document Loading:
Loads and extracts text from the PDF document.

### Summarization:
Summarizer agent generates a concise summary.

### Review:
Reviewer agent critiques the generated summary for accuracy and completeness.

### Iteration:
If user feedback is provided, the summarizer refines the output based on critique.

### Visualization:
The summarization-review loop is visualized using a Mermaid Diagram.

## 📷 Agent Flow Diagram

![image](https://github.com/user-attachments/assets/af8dec96-6d08-4e38-ae8b-a45deb92291c)


🧠 Technologies Used
  - LangChain
  - LangGraph
  - Groq Inference Engine
  - Huggingface Embeddings
  - PyPDFLoader
  - Google Colab

## ✨ Future Enhancements
  - ✅ Add support for multi-page documents

  - ✅ Allow dynamic model selection (e.g., smaller Groq models)

  - ✅ Build a Streamlit UI for broader usability

  - ✅ Fine-tune summarization length and style settings

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.

## 📬 Contact
For questions, suggestions, or collaborations:
Mohamed — shaadclt@gmail.com



<h1 align="center">Chat with PDF using Llama3</h1>
<h2 align="center">Introduction</h2>
A simple Streamlit app interface that answers questions about an uploaded PDF document via Llama3.

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://rag-based-chat-with-pdf-using-llama3.streamlit.app/)

<img  align="right" height=290 width=510 src="https://docs.aws.amazon.com/images/sagemaker/latest/dg/images/jumpstart/jumpstart-fm-rag.jpg" />

 This project implements a chat interface that allows users to ask questions about uploaded PDF documents. It leverages a Retrieval-Augmented Generation (RAG) approach, combining:

- Information Retrieval: Efficiently searching relevant passages in the PDF content using FAISS and text embeddings.
- Generative Language Model (LLM): Answering user questions in a comprehensive and informative way using Llama3, a large language model from Google AI for embeddings.

<h2 align="center">Features</h2>

- Upload multiple PDF documents.
- Ask questions about the content of the uploaded PDFs.
- Get answers generated by Llama3 based on the retrieved information.

<h2 align="center">Requirements</h2>

- Python 3.x
- Streamlit
- PyPDF2
- langchain
- langchain_community
- langchain-groq (Groq API access)
- langchain-google-genai (Google Generative AI access)
- dotenv (for environment variables)

<h2 align="center">Installation </h2>

1. Install the requirements

   ```
   $ pip install -r requirements.txt
   ```

2.  Set up your Groq API key and Google Cloud project credentials
    ```
    GROQ_API_KEY=your_groq_api_key
    GOOGLE_API_KEY=your_google_api_key
    ```
    
3.  Run the app

    ```
    $ streamlit run streamlit_app.py
    ```

4.  Upload your PDF files in the sidebar.
5.  Click the "Submit & Process" button.
6.  Once processing is complete, enter your question in the text box.
7.  Click "Enter" to receive an answer generated by Llama3 based on the uploaded PDFs.    
    
<h2 align="center">Use Cases </h2>
Research and Document Summarization:

- Students and researchers can upload research papers, articles, or reports and ask specific questions about the content.
- The chat interface can summarize key findings, identify relevant sections based on the question, or provide supporting evidence from the document.
  
Legal Document Analysis

- Lawyers or legal professionals can upload contracts, agreements, or court documents and ask clarifying questions about terms, clauses, or procedures.
- The chat can highlight relevant sections, identify potential ambiguities, or offer preliminary interpretations based on the document's content.
  
Technical Documentation Exploration

- Software developers, system administrators, or technical support personnel can upload user manuals, technical specifications, or troubleshooting guides.
- The chat can answer questions about specific features, configuration options, or troubleshooting steps based on the information within the documents.
  
Customer Service Chatbots

- Companies can leverage this technology to build chatbots that answer customer questions about product manuals, FAQs, or service policies.
- Users can upload relevant documents and get immediate, context-aware responses based on the retrieved information.

 Educational Materials and Assistive Technologies

- Students with learning disabilities can upload educational materials and ask questions about specific concepts or passages.
- The chat can provide paraphrased explanations, offer alternative learning resources, or highlight key points from the document.
    
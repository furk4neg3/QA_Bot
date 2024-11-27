# RAG Chatbot for PDF Question-Answering with IBM Watsonx and LangChain  

This project demonstrates a Retrieval-Augmented Generation (RAG) chatbot that allows users to upload PDF documents and ask questions. The chatbot provides answers using the contents of the uploaded PDF, leveraging IBM Watsonx's powerful LLM and embedding models along with LangChain for document processing and retrieval.

## Key Features  
- **Question-Answering from PDFs:** Upload a PDF, ask a question, and get an answer based on the document's content.  
- **Retrieval-Augmented Generation (RAG):** Combines document retrieval and generative models to provide accurate responses.  
- **LangChain Integration:** Utilizes LangChain for text splitting, document loading, and vector database management.  
- **Gradio Interface:** Provides an interactive web interface for easy user interaction.  

## Objectives  
- Implement document loader to extract text from PDFs.  
- Use text splitting techniques to handle large documents.  
- Employ Watsonx for embeddings and LLM inference.  
- Set up a vector database to store document embeddings.  
- Build a question-answering system using the retrieval-augmented generation (RAG) approach.  
- Create a Gradio interface to make the chatbot user-friendly.

## Workflow
- Document Loader: The PDF file is loaded using PyPDFLoader from LangChain.
- Text Splitter: The document is split into smaller chunks using RecursiveCharacterTextSplitter.
- Embedding: Each chunk is embedded using Watsonx's embedding model (ibm/slate-125m-english-rtrvr).
- Vector Database: The chunks are stored in a vector database (Chroma) for efficient retrieval.
- Retriever and QA Chain: The chatbot uses the retriever to find relevant information and the LLM to generate an answer.

## Example Interaction
- Upload a PDF document containing your desired information.
- Ask a question, such as "What is the main topic of the document?"
- Receive a generated response based on the content of the uploaded PDF.
  
## Requirements
- Python 3.x
- Gradio
- LangChain
- IBM Watsonx SDK
- Chroma (vector store)

# Chatbot-Context-Aware

This project implements a context-aware chatbot that can answer questions based on a custom CSV corpus. It retrieves relevant information using a FAISS vector store and generates responses using a Hugging Face FLAN-T5 model.

Features

Processes text to remove punctuation, stopwords, and lowercase all content.

Splits large text into smaller chunks for better retrieval.

Converts text into vector embeddings using sentence-transformers.

Efficiently stores and searches chunks using FAISS.

Generates context-aware responses using FLAN-T5.

Maintains conversation history for multi-turn interactions.

Allows clearing of chat history.

Technologies Used

Python 3.12

Pandas – Data handling

NLTK – Text preprocessing

LangChain Community – Embeddings, FAISS, LLM integration

Sentence-Transformers – Text embeddings

Streamlit – Chat interface and deployment

Hugging Face FLAN-T5 – Large language model for text generation

Setup Instructions

Prepare a CSV corpus containing text for the chatbot.

Create a Hugging Face account and generate a Read token.

Configure the project to use the Hugging Face token for the model.

Preprocess the corpus, generate embeddings, and create a FAISS index.

Launch the interactive chatbot using Streamlit.

How It Works

User Input – The user enters a question.

Retrieval – Top relevant chunks are retrieved from the FAISS vector store.

Answer Generation – The FLAN-T5 LLM generates a response based on the retrieved context.

Display – The chatbot shows the response and maintains the conversation history.

# Experiment 12: RAG Data Indexing and Retrieval Using FAISS

## Aim
To build a basic data indexing pipeline for Retrieval-Augmented Generation (RAG) by splitting a text document into chunks, generating embeddings, storing them in FAISS, and retrieving relevant chunks using similarity search.

## Problem Statement
Create a Python pipeline that indexes a sample climate change document and retrieves the two most relevant chunks for a user query.

## Tools and Technologies
- Python
- Google Gemini API
- LangChain
- Gemini embeddings
- FAISS vector store
- Google Colab

## Algorithm
1. Install the required packages.
2. Configure the Gemini API key.
3. Define a sample text about climate change.
4. Split the text using `RecursiveCharacterTextSplitter`.
5. Use a chunk size of 300 characters and overlap of 30 characters.
6. Generate embeddings using `GoogleGenerativeAIEmbeddings`.
7. Create the vector store using `FAISS.from_documents()`.
8. Search for the two most relevant chunks using `similarity_search_with_relevance_scores()`.
9. Print the retrieved chunks and relevance scores.
10. Save the results to `output.txt`.

## Query
What are the effects of climate change?

## Expected Output
- Number of chunks created.
- The query used for retrieval.
- The top two relevant text chunks.
- A relevance score for each retrieved chunk.

## Conclusion
The experiment demonstrates how text chunking, embedding generation, vector storage, and similarity search can form the indexing and retrieval components of a RAG system.

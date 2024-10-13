# Medical Chatbot Using Pinecone and LLaMA2

This project is a **medical chatbot** designed to assist users with healthcare-related queries. It integrates **Pinecone** as a vector database to perform sequential search and uses **LLaMA2** to generate detailed, human-like responses. The workflow involves searching the medical knowledge base using vector similarity, retrieving relevant documents, and then passing the results to LLaMA2 for final response generation.

## Features

- **Vector-based Search with Pinecone**: Pinecone is used to perform fast, semantic search on large medical document databases, ensuring relevant information is retrieved.
- **LLaMA2 for Response Generation**: The retrieved information is processed by **LLaMA2**, a state-of-the-art language model, to generate accurate and conversational responses.
- **Sequential Search**: After the user query is embedded, a sequential search is done through Pinecone, and the retrieved documents are passed to the LLaMA2 model for response generation.
- **Medical Knowledge Base**: The bot is equipped with a database of medical information, capable of responding to queries related to symptoms, treatments, diseases, and general health advice.
- **Contextual Conversations**: The chatbot can handle follow-up questions and retain the context of the conversation for multi-turn dialogues.
- **Scalable and Efficient**: Pinecone allows the system to scale easily for large datasets while ensuring high performance in query retrieval.

## How It Works

1. **User Query**: The user submits a healthcare-related question or symptom query.
2. **Vector Search**: The query is embedded and a vector-based search is performed using Pinecone to retrieve the most relevant medical documents.
3. **LLaMA2 Processing**: The retrieved documents are passed to the LLaMA2 model, which generates a natural language response based on the information.
4. **Final Response**: The chatbot provides the final response back to the user, offering a clear and informative answer to their query.

## Project Workflow

1. **Data Ingestion**: Medical documents are pre-processed, embedded, and indexed in Pinecone.
2. **Query Embedding**: When a user inputs a query, it is embedded into a vector representation.
3. **Search and Retrieval**: A sequential search is conducted in Pinecone to retrieve relevant documents based on vector similarity.
4. **Response Generation**: The search results are passed to the LLaMA2 model to generate a coherent and accurate response.
5. **Return Response**: The chatbot delivers the response to the user in a conversational format.



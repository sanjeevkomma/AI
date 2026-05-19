# ToRead
* RAG = Retrieval-Augmented Generation
* RAG is a framework where a language model retrieves relevant external data (documents, PDFs, database info, etc.) and generates answers based on that data, rather than relying solely on what it was trained on

# RAG Workflow – Step-by-Step
1. User Query
    * Example: "What are the side effects of Metformin?"
2. Retriever
    * Searches external sources (e.g., medical documents, knowledge base, vector DB like Pinecone or FAISS) to find relevant chunks.
    * Usually uses semantic search or embeddings.
3. Reader / Generator (LLM)
    * Takes the user query + retrieved documents and generates a final, context-aware answer.
  
# Diagram (Simplified)
* User Question → [Retriever] → Relevant Documents → [Generator (LLM)] → Answer

# Tech Stack Used
|#Component| #Example Tools |
| :---| :--- | 
|Embeddings |  OpenAI, HuggingFace, Cohere |
|Vector Store |  FAISS, Pinecone, Weaviate, Chroma | 
|LLM |  OpenAI GPT, Mistral, Claude, LLaMA | 
|Frameworks |  LangChain, LlamaIndex, Haystack | 

# Why Use RAG?
* Adds fresh knowledge to models (without fine-tuning)
* Keeps data private & up-to-date
* Reduces hallucinations
* Ideal for enterprise search, customer support, legal, healthcare, etc.

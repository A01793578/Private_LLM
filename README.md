## RAG-based Question Answering System

This repository contains a Python implementation of a Retrieval-Augmented Generation (RAG) system for question answering. The system leverages a vector store (ChromaDB) to retrieve relevant documents and a powerful language model (LlamaCpp or GPT4All) to generate answers.

**Features:**

* **Data Loading & Preprocessing:** Supports loading and splitting documents from various file types, including CSV files.
* **Embeddings & Vector Store:**  Uses Hugging Face embeddings to create vector representations of text chunks and stores them in a ChromaDB vector store.
* **Retrieval:** Efficiently retrieves relevant documents based on user queries using the Chroma retriever.
* **Language Models:** Offers support for both LlamaCpp and GPT4All language models.
* **Question Answering:** Combines retrieval and language modeling to generate answers grounded in relevant context.
* **Evaluation:** Includes prompts and metrics for evaluating the system's performance on context relevance, groundedness, and answer faithfulness.

**Getting Started:**

1. **Install Dependencies:**
   ```bash
   pip install langchain gpt4all chromadb llama-cpp-python urllib3 python-dotenv tqdm sentence_transformers langchain-community
   ```

2. **Configure Settings:**
   * **`source_directory`:** Path to the directory containing your training data.
   * **`model_path`:** Path to the directory containing your language model (LlamaCpp or GPT4All).
   * **`persist_directory`:** Directory where the vector store will be persisted.
   * **`embeddings_model_name`:** Name of the Hugging Face model used for embeddings (e.g., `all-MiniLM-L6-v2`).

3. **Run the Code:**
   ```bash
   python avance5_39.py
   ```

**Example Usage:**

The code includes example prompts and expected answers for testing the system. You can modify these prompts to explore different question types.

**LLM Location :**

* **Llama 2:** https://drive.google.com/file/d/1IT7sO5WVazay0jsAe1rEi4U84UZV2bc_/view?usp=sharing
* **GPT:** https://drive.google.com/file/d/18tpUVBzJakoSmw-dXBfS849BU0xvSx0p/view?usp=sharing

**Further Learning:**

* **LangChain Documentation:** [https://python.langchain.com/v0.1/docs/integrations/llms/llamacpp/](https://python.langchain.com/v0.1/docs/integrations/llms/llamacpp/)
* **RAG Triad Introduction:** [https://medium.com/@rajib76.gcp/rag-triad-introduction-4e5ecba26741](https://medium.com/@rajib76.gcp/rag-triad-introduction-4e5ecba26741)
* **Evaluating RAG Applications:** [https://towardsdatascience.com/evaluating-rag-applications-with-ragas-81d67b0ee31a](https://towardsdatascience.com/evaluating-rag-applications-with-ragas-81d67b0ee31a)

**Contributions:**

Contributions to this project are welcome! Please feel free to open issues or submit pull requests.

**License:**

This project is licensed under the MIT License.

**Note:** This README file is a template. You can customize it further to provide more detailed information about your project and its functionality.

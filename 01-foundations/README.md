# Retrieval-Augmented Generation
## What is RAG?
RAG is about using a Large-Language Model (LLM) for answering question about some previously unseen data.
LLMs are typically trained on large public datasets and do not have knowledge of private databases.

With RAGs, you give the LLM access to a basis of knowledge that you own and want the LLM to answer questions about.
The knowledge base base form a __context__ used by the LLM to provide precise and accurate answers to user-supplied questions.

## Data pipeline
The knowledge based used by RAG systems is made available to an LLM by placing it into a search engine.
A __data pipeline__ is a piece of code that extracts, transforms and loads some data into a search engine.

When a user submits a question, the RAG system identifies the relevant documents via the search engine.
The user question and retrieved documents are then combined to form a __prompt__. This prompt is passed to the LLM, which outputs a context-aware response back to the user.

A proper data pipeline is a preparatory step that enables the RAG flow by updating the search engine.
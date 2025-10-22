# Retrieval-Augmented Generation
## The limits of LLMs
Large Language Models (LLMs) are trained using large quantities of publicly available data. This data forms the knowledge base on which the model relies to provide answers to user prompts.

In many practical applications, we want to use LLMs to answer questions about specific material that is not part of this public knowledge base. In order for an LLM to be of any use to any such application, it needs to be provided case-specific data on which to base answers.

The adhoc knowledge passed to an LLM is often referred as *context*. The quality of an AI application is highly dependent on the appropriate context being passed to the underlying LLM. Retrieval-augmented generation (RAG) is a framework for retrieving relevant information and passing it on to an LLM.

## What is RAG?
Retrieval-Augmented Generation is a commonly used application that allows users to interact with proprietary information through a publicly-trained LLM.

Say an online course platform has an FAQ document available only to paid subscribers. Developers may want to create an AI chatbot that user can turn to instead of parsing through the document. In order for the underlying LLM to provide usefule and accurate answers, the document content is passed to the LLM along with every user query.

In a RAG system, a search engine uses the user query to identify relevant documents in the knowledge base (retrieval part). This subset of documents is what is ultimately passed to the LLM for context. By preemptively narrowing the scope of the information that the LLM has to work with, we reduce the risk of incorrect responses and make the process more cost-effective. Naturally, he quality of RAG's information pre-selection system has an important impact on the quality of the LLM responses.

## The RAG flow
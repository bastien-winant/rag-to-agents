# Retrieval-Augmented Generation
## The limits of LLMs
Large Language Models (LLMs) are created using large quantities of publicly available data. This data forms the knowledge base on which the model relies to provide answers to user prompts.

In many practical applications, we want to use LLMs to answer questions about specific material that is not part of this public knowledge base. In order for an LLM to be of any use to any such application, it needs to be provided case-specific data on which to base answers.

The adhoc knowledge passed to an LLM is often referred as *context*. The quality of an AI application is highly dependent on the appropriate context being passed to the underlying LLM. Retrieval-augmented generation (RAG) is a framework for retrieving relevant information and passing it on to an LLM.

## What is RAG?
Retrieval-Augmented Generation is a framework by which an LLM is given access to an external knowledge base

## The RAG flow
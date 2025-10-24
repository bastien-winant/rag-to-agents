# Vector Search
## Text vs Semantic Searching
Text-based searching works by looking for matching keywords between the search term and the document base.
It is often for many RAG applications, but some cases require approximate searching based on semantics rather than exact matches.

Vector search (semantic search) addresses this need by turning text into vectors. The transformations is such that
semantically similar words produce vectors that are close in space.

## Chunking
The documents used in a RAG system may be large, leading to inefficient and expensive LLM queries.
It is often more effective to index large documents and use a search engine to retrieve only the most relevant parts of the document to be passed to the LLM.

Chunking is the process of splitting a large document into sequential subparts. In order to limit context loss and missing connections, we want to ensure adjacent subparts have some overlap.

When chunking a large monolithic document, the following must be defined:
- __size:__ the size of each junk window (expressed in number of characters, bytes, etc.)
- __step:__ the size of the shift to the next window (the smaller the step, the higher the overlap)
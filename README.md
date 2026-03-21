# Generative Doc Search

This is a generative search system capable of effectively and accurately answering questions from a Group Member Life Insurance Policy document.

The project comprises of following three layers in order to build an effective search system:

**The Embedding Layer:** The insurance document needs to be effectively processed, cleaned, and chunked for the embeddings.

**The Search Layer:** Here, you first need to design at least 3 queries against which you will test your system. You need to understand and skim through the document, and accordingly come up with some queries, the answers to which can be found in the policy document. Here we embed the search queries and search ChromaDB vector database against each of these queries. A cache mechanism is also implemented to handle the load. Finally, there is a re-ranking block implemented using cross-encoding model.

**The Generation Layer:** In the generation layer, the final prompt design is the major component. Here we make sure that the prompt is exhaustive in its instructions, and the relevant information is correctly passed to the prompt.

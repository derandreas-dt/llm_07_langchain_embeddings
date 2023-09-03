This is the first embedding script, that loads simple text documents
into a vector store and enhances the LLM model with new informations.
To run this, chromadb needs to be installed.

This uses standard llama embeddings and chromadb (pip install chromadb)
For testing this, the plain LLM is asked for the CEO of Twitter.
In the next example, the RetrievalQA is used, with two additional texts:
    1. Elon Musk is new CEO
    2. Lina Yaccarino is new CEO

One text is english and one is german.

(Note the texts are in order of the date, if not it is wrong!)

The reults are:

```
Anwer without langchain embeddings to the question: Who is CEO of twitter?
As of March 2023, Twitter's CEO is Jack Dorsey. He co-founded Twitter and has been the CEO twice, first from 2006 to 2008 and again since 2015.
Context: You are looking for information about the CEO of Twitter.

Answer with Langchain embeddings to the question Who is CEO of twitter?
On 01.07.2023, it was announced that Linda Yaccarino would be the new CEO of Twitter. So, the answer is Linda Yaccarino.
```

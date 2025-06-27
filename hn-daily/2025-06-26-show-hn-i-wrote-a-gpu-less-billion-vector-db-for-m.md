# Show HN: I wrote a GPU-less billion-vector DB for molecule search (live demo)

**Posted by mireklzicar on 2025-06-26**

I developed a system that allows you to input a SMILES string (or select from example molecules) and retrieves up to 100,000 molecules closest in 3D shape or electrostatic similarity from a database exceeding 10 billion entries. The query process typically completes in under 5-10 seconds.

### Why it might interest HN

- The entire index resides on **disk** — there is no need for GPU at query time, and it requires less than ~10 GB of RAM total.
- Built from scratch without relying on FAISS, Milvus, Pinecone, or similar indexing solutions.
- The index-building cost is approximately one Nvidia T4 (around $300) for a 5.5-billion-molecule database.
- Open to everyone: useful for predicting ADMET properties, and results can be exported as CSV or SDF files.

### Further details

A full write-up and benchmark results (using datasets like DUD-E, LIT-PCBA, and SVS) are available in the pre-print:

[https://chemrxiv.org/engage/chemrxiv/article-details/67250915f9980725cfcd1f6f](https://chemrxiv.org/engage/chemrxiv/article-details/67250915f9980725cfcd1f6f)
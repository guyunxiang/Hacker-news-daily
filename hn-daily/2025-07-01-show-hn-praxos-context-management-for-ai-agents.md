# Show HN: Praxos – Context Management for AI Agents

**Posted by mogusian on 2025-07-01**

Hey HN! We're Lucas and Soheil, the founders of Praxos ([praxos.ai](https://praxos.ai)). Praxos is a context manager for AI agents, providing everything you need to build stateful agents that don’t break in production.

---

## What is Praxos?

Praxos can parse any data source—unstructured PDFs, API streams, conversational messages, structured databases—and transform them into a single Knowledge Graph. Every element in this graph is semantically typed, and relationships are explicit, turning raw data into a clean, queryable universe of understanding that AI can utilize accurately.

Whether you need to query for specific answers or extract data aligned with your use case, Praxos handles it all without requerying. This allows AI applications to process data end-to-end and act on it through single-chain or multi-chain reasoning steps. Intermediate, final, and user-edited outputs can be added back into the knowledge graph, enabling Praxos to learn dynamically.

---

## Why We Built Praxos

During our work in insurance, we encountered two major challenges deploying AI:

1. **Document Parsing Limitations:**  
   LLMs struggled to parse complex documents like property schedules and insurance policies—often consisting of 50+ pages across Word, Excel, and PDF. These documents contain detailed, interconnected data about physical properties, but recreating a semantic model was difficult. As a result, relationship information was lost, left blank, or hallucinated.

2. **Cascading Errors in Data Handling:**  
   Repeatedly searching, retrieving, and updating information led to cascading errors, especially across complex tasks such as reading documents, fetching previous user data, performing calculations, and presenting results. This fragmentation compromised accuracy and reliability.

We realized that making relationships explicit is key. Much of the contextual information is implicit and not directly accessible programmatically. Without explicit relationships, LLMs have to interpret everything anew each time, leading to errors.

This insight motivated us to build Praxos—to provide a robust, explicit context management system that makes data relationships clear and accessible.

---

## How Praxos Works

We offer a self-serve option with a free tier (up to a data cap) suitable for hobbyists and early adopters. For context—this tier covers about 200 document pages. You can sign up here: [https://data.praxos.ai/sign-up](https://data.praxos.ai/sign-up).

Our first release is an SDK designed to meet all your data extraction, retrieval, and updating needs.

### Key Features:

- **Organizing Information:**  
  Praxos structures data into ontologies—schemas that define types, attributes, and relationships—guiding how the knowledge graph is built and interpreted.

- **Processing Input Data:**  
  It can handle any data source—PDFs, tables, JSON, conversational data—and performs extraction seamlessly. No need for OCR, chunking, or pre-processing; just pass in the file and select your ontology.

- **Retrieving Information / Memories:**  
  For each query, Praxos searches related stored info using graph traversal, vector similarity, and key-value lookups. It returns entities, their connections, and relevant sentence snippets.

---

## Join the Conversation!

We’re eager to hear your feedback. Feel free to explore Praxos, and share your thoughts or suggestions on our Discord: [https://discord.gg/wVmrXD2dJA](https://discord.gg/wVmrXD2dJA).

Your input will help shape the future direction of Praxos!
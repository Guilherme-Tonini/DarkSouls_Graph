# Use of AI Tools in This Project

Throughout this project, artificial intelligence (AI) tools, specifically OpenAI's ChatGPT, were used to assist in the following key tasks:

## 1. Queryng

To streamline the workflow and ensure greater reusability, advanced functions were developed in collaboration with ChatGPT. These functions consolidate multiple processing steps into single, well-structured queries. Instead of writing repetitive code blocks across different cells in a Jupyter Notebook, each function was designed to perform a complete task from end to end. This approach not only improves efficiency and readability but also makes the analysis pipeline easier to maintain and scale.

Moreover, the project provided an opportunity to explore and learn about graph query design, an area that was previously unfamiliar. With guidance and iterative refinement using ChatGPT, customized queries for knowledge graph exploration and entity-relationship retrieval were developed

## 2. Entities and Relations

ChatGPT was employed as a key tool for interpreting item descriptions and dialogue texts due to its advanced natural language capabilities. By leveraging a language model trained on public textual data, including content related to the Dark Souls universe, ChatGPT was able to:

-Detect named entities with contextual adaptation
-Interpret text semantically and pragmatically
-Disambiguate terms with multiple meanings
-Apply regex-based pattern recognition
-Identify characters, terms, and references not yet catalogued
-Suggest meaningful relationships between entities

This allowed for the dynamic expansion of the entity database by uncovering hidden or implicit references and relationships that might be missed through traditional rule-based methods alone.

## Automation

ChatGPT was instrumental in automating key steps of the knowledge graph pipeline. Once entities and their relationships had been extracted and organized, ChatGPT was used to generate .graphml files for seamless import into graph visualization tools. Additionally, it produced well-structured .csv files for nodes and edges, tailored for direct integration with Neo4j Aura.


# Weighted Knowledge Graph Representation

## Overview
This repository contains an implementation of a **Knowledge Graph with Weighted Edges**, where the edge thickness represents the frequency of relationships between entities. The project is inspired by **Google’s Knowledge Graph** ([Google Blog](https://blog.google/products/search/introducing-knowledge-graph-things-not/)), which shifted search from keyword-based retrieval to entity-based structured knowledge.

## Motivation
The objective of this project is to:
- Build a **Knowledge Graph** using **Python, NLP, and NetworkX**.
- Implement **edge weights** based on relationship frequency.
- Sample **100 nodes** for a readable subgraph.
- Improve the **representation of relationships** between entities by incorporating weighted visualization.

## Dataset
The dataset used is **wiki_sentences_v2.csv**, obtained from a Kaggle project: [Build Knowledge Graph using Python](https://www.kaggle.com/code/nageshsingh/build-knowledge-graph-using-python). It contains textual data from Wikipedia, which is parsed and structured into a knowledge graph.

## Features
- **Entity Extraction** using [[spaCy NLP models]] ([spaCy](https://spacy.io)).
- **Relation Identification** from textual data.
- **Graph Construction** using [[NetworkX library]] ([NetworkX](https://networkx.github.io)).
- **Weighted Edges**: The frequency of relationships is used to determine the thickness of edges.
- **Graph Sampling**: A subset of **100 nodes** is used to visualize a readable graph.
- **Scalability**: The implementation is scalable for larger datasets.

## Implementation Details
The project involves the following steps:
1. **Preprocessing Text Data**: Tokenizing and cleaning Wikipedia sentences.
2. **Extracting Entities & Relations**: Using spaCy and custom parsing methods.
3. **Building the Graph**: Using NetworkX to create nodes (entities) and edges (relationships).
4. **Computing Edge Weights**: Counting the frequency of relationships in the dataset.
5. **Visualizing the Graph**: Using matplotlib to plot the graph with weighted edges.
6. **Sampling 100 Nodes**: To generate a clear and interpretable subgraph.

## Output Visualization
Below is an example output of the **Weighted Knowledge Graph**:

![Knowledge Graph Output](https://github.com/om-umrania/Weighted-Knowledge-Graph-Representation/blob/main/Building%20Knowledge%20Graph%20Using%20Python%20with%20200%20Weighted%20Relation.png.png)


This visualization shows the **weighted relationships** between entities, where edge thickness represents the frequency of occurrence in the dataset.

## Code Usage
### Prerequisites
Install the necessary dependencies:
```sh
pip install spacy numpy pandas networkx matplotlib tqdm
python -m spacy download en_core_web_sm
```

### Running the Code
```sh
python knowledge_graph.py
```

## Impact
The implementation has significant implications for:
- **Knowledge Representation**: Capturing and structuring unstructured data efficiently.
- **Search Engines**: Enhancing information retrieval by moving from string-based searches to entity-based searches.
- **Recommendation Systems**: Understanding user behavior through linked entities.
- **Healthcare & AI Research**: Applying knowledge graphs to medical records for diagnosis prediction.

## Learnings & Future Enhancements
### Key Takeaways
- Knowledge Graphs are **crucial for structuring data** in a meaningful way.
- **Google’s approach in 2012** remains **relevant today** in AI-driven systems like LLMs.
- **Weighted relationships improve accuracy** in graph-based inference tasks.
- **Graph sampling helps readability**, avoiding overly complex visualizations.

### Future Improvements
- **Dynamic Updates**: Implementing real-time knowledge graph updates.
- **Multi-Modal Knowledge Graphs**: Incorporating images, videos, and structured data.
- **Neural Graph Embeddings**: Applying GNNs for better entity representation.
- **Scalable Implementations**: Using **Neo4j** for enterprise-level graph processing.

## Repository Links
- **GitHub Repository**: [Weighted Knowledge Graph Representation](https://github.com/om-umrania/weighted-knowledge-graph)
- **Kaggle Notebook**: [Build Knowledge Graph](https://www.kaggle.com/code/nageshsingh/build-knowledge-graph-using-python)

## References
- [Google Knowledge Graph Introduction](https://blog.google/products/search/introducing-knowledge-graph-things-not/)
- [Alan Turing Institute’s Knowledge Graph Research](https://www.turing.ac.uk/research/interest-groups/knowledge-graphs)
- [Kaggle: Building a Knowledge Graph](https://www.kaggle.com/code/nageshsingh/build-knowledge-graph-using-python)

## Author
Om Umrania  
[LinkedIn](https://www.linkedin.com/in/omumrania/) | [GitHub](https://github.com/om-umrania)




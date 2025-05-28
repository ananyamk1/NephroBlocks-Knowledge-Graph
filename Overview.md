## **📂 Project_Overview.md**

# Project Overview: Neo4j-Based Clinical Trial Knowledge Graph

## Introduction
Medical research relies heavily on **structured data** for informed decision-making. Clinical trial insights are often fragmented across multiple sources, making it challenging to **connect trial procedures with relevant patient profiles**. This project **aims to bridge this gap** by leveraging **graph database technology** and **machine learning** to structure nephrology clinical trial data.

## Architecture
### 🔹 **Data Collection**
- **Web scraping** using BeautifulSoup to extract clinical trial research papers.
- **CSV file creation** storing extracted information like **Title, Authors, Category, Drugs, Treatments, and Disease Type**.

### 🔹 **Text Processing**
- **Tokenization & Stopword Removal** (NLTK).
- **TF-IDF vectorization** to extract keywords from research papers.

### 🔹 **Machine Learning for Classification**
- **K-means clustering** to categorize research papers into disease-related clusters.
- **GPT-3-powered Cypher queries** for automated Neo4j search.

### 🔹 **Neo4j Graph Database Setup**
- **Nodes Created**: Paper, Author, Disease, Drugs, Treatments, Type.
- **Relationships Established**: `IN_CATEGORY`, `AUTHORED`, `DRUG_LABEL`, `TREATMENT_LABEL`.

## Results & Impact
-> **Reduced manual review time for nephrology literature by 70%**  
-> **Connected 496+ research papers to structured patient-trial data**  
-> **Enabled intelligent querying using NLP-powered search**

## Future Scope
- **Integrating privacy-preserving federated learning** for secure trial data sharing.
- **Expanding database connections** with additional clinical domains.

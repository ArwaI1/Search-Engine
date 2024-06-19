
# Information Retrieval System Project

## Overview

This project focuses on developing an advanced Information Retrieval (IR) system utilizing the CISI dataset. The main goal is to create a search engine capable of efficiently processing and retrieving relevant documents in response to user queries. The project leverages the BM25 algorithm for ranking documents and includes a comprehensive evaluation of the system's performance using key metrics such as precision, recall, and response time.

 **data/**: Directory containing the CISI dataset files:
  - `CISI.ALL`: Document collection.
  - `CISI.QRY`: Query set.
  - `CISI.REL`: Relevance judgments.
- **IR_PROJECT.ipynb**: Jupyter notebook with the project's code and documentation.
- **README.md**: This file, providing an overview and instructions.

## Installation

### Prerequisites

- Python 3.x
- Jupyter Notebook

### Steps

1. **Clone the Repository**

   ```sh
   git clone <repository_url>
   cd IR_PROJECT
   ```

2. **Install Dependencies**

   Use pip to install the required Python packages:

   ```sh
   pip install pandas pyterrier
   ```

## Dataset

The project utilizes the CISI dataset, which includes:

- **CISI.ALL**: Contains the documents.
- **CISI.QRY**: Contains the queries.
- **CISI.REL**: Contains relevance judgments for evaluation.

## Usage

1. **Open the Jupyter Notebook**

   Start Jupyter Notebook and open `IR_PROJECT.ipynb`:

   ```sh
   jupyter notebook IR_PROJECT.ipynb
   ```

2. **Run the Notebook**

   Execute the cells in the notebook sequentially. The notebook guides you through:
   - Reading and preprocessing documents from `CISI.ALL`.
   - Reading and preprocessing queries from `CISI.QRY`.
   - Reading and preprocessing relevance judgments from `CISI.REL`.
   - Implementing the BM25 algorithm for ranking.
   - Defining and executing search and evaluation functions.

3. **Search and Evaluate**

   Utilize the provided functions to input search queries and assess the search engine's performance using precision, recall, and response time metrics.

## Functions Overview

- **read_documents(documents_path)**: Reads and processes documents from the provided path.
- **read_queries(queries_path)**: Reads and processes queries from the provided path.
- **read_qrels(qrels_path)**: Reads and processes relevance judgments from the provided path.
- **search(query, bm25_model)**: Performs a search using the BM25 model and returns ranked documents.
- **evaluate_search_engine(query, search_func, doc_df)**: Evaluates the search engine's performance based on the given query.

## Evaluation Metrics

- **Precision**: Measures the accuracy of the retrieved documents.
- **Recall**: Measures the completeness of the retrieved documents.
- **Response Time**: Measures the time taken to process and return search results.


## S&P 100 Company Information Extraction and Analysis

### Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Setup Instructions](#setup-instructions)
4. [Replicability](#replicability)
5. [Project Components and Technologies](#project-components-and-technologies)

## Introduction
This project consists of three Python notebooks: `10-Scraper.ipynb`, `20-Queries.ipynb`, and `30-RAG.ipynb`. It is designed to scrape financial data from the SEC's EDGAR database, perform advanced queries on the data, and generate a Retrieval Augmented Generation (RAG) model using OpenAI's embedding model and large language model.

## Features
- **Data Scraping**: Automated extraction of financial statements and metadata from EDGAR.
- **Data Querying**: Execution of seven unique queries to extract desired information from MongoDB.
- **RAG Model Generation**: Implementation of a Retrieval Augmented Generation model for enriched data interpretation.

## Setup Instructions
1. **Clone Repository**:
   - Clone the repository to your local machine.

2. **Install Required Libraries**:
   - Install the required Python libraries by running `pip install -r requirements.txt` in your terminal.

3. **MongoDB Setup**:
   - Ensure MongoDB is installed and running. Configure the MongoDB connection in both `10-Scraper.ipynb` and `20-Queries.ipynb`.

4. **OpenAI API Key**:
   - For `30-RAG.ipynb`, set the OpenAI API key as an environment variable:
     ```bash
     export OPENAI_API_KEY='your_api_key_here'
     ```

5. **Run Notebooks**:
   - Open and execute the cells in each notebook using a Jupyter environment.

## Replicability
Follow the setup instructions for easy replication of the project. Ensure all dependencies are installed and MongoDB and OpenAI API key are configured correctly.

## Project Components and Technologies

This project leverages a variety of technologies and resources to achieve its objectives. Below is a list of the key components used:

- **SEC EDGAR System**: Used for scraping financial documents, from the Securities and Exchange Commission's database.

- **OpenAI Models**: Utilization of OpenAI's models, including GPT (Generative Pretrained Transformer) base models and the `text-embedding-ada-002` for embedding generation.

- **ChromaDB**: Employed as a vector database to store and manage vector embeddings.

- **Websites for Data Scraping**:
  - [Liberated Stock Trader](https://www.liberatedstocktrader.com/sp-500-companies/): Source for scraping the top 100 S&P 500 companies by market capitalization general information.
  - [Wikipedia - List of S&P 500 companies](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies): Utilized for additional information regarding S&P 500 companies.

- **MongoDB Atlas**: Used as the primary database for storing and querying the scraped data.

- **Langchain Framework**: Employed for the development of the Retrieval Augmented Generation (RAG) model.

- **JSON (JavaScript Object Notation)**: For handling data in a lightweight data-interchange format.

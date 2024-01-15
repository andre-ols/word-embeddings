# iBeer Recommender System

## Overview

This project involves creating a beer recommendation system based on word embeddings. The system utilizes Natural Language Processing (NLP) techniques to analyze beer descriptions and user queries, providing personalized beer recommendations.

## Installation

Before running the code, ensure you have the required Python packages installed. You can install them using the following command:

```bash
pip install pandas openai
```

## Data

The beer information is stored in a CSV file named `beers.csv`. The dataset includes details such as beer name, category, ABV (Alcohol By Volume), IBU (International Bitterness Units), EBC (European Brewery Convention), food pairings, and a brief description.

## Workflow

The workflow for this project is as follows:

1. **Loading Data**: The beer dataset is loaded into a Pandas DataFrame.

2. **Text Summary Generation**: A function named `summary` is defined to generate a textual summary for each beer based on its attributes.

3. **Embedding Generation**: The OpenAI Embedding API is used to generate embeddings for each beer summary.

4. **Cosine Similarity Calculation**: A function for cosine similarity is defined to measure the similarity between user queries and beer embeddings.

5. **User Interaction**: The system prompts the user for beer-related queries.

6. **Recommendation Generation**: Based on user input, the system computes the similarity between user queries and beer summaries, providing a list of recommended beers along with their descriptions.

## Chat-based Recommendation

The project includes an additional feature where users can interact with the system in a chat format. The send_question function prompts users for questions, generates context for chat-based completion, and uses OpenAI GPT-3.5 Turbo for response generation.

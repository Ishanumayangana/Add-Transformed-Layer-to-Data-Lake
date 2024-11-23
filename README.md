# Adding Transformed Layer to Data Lake Project

## Problem Statement
This project involves building a basic **Data Lake** in Python. The goal is to implement a data processing pipeline with multiple layers, where each layer performs specific data operations and saves the results in a structured manner.

Additionally, a new layer named **"Transformed"** is added to the pipeline. This layer applies specific data transformations to enrich the dataset.

## Layers and Operations

| **Layer**      | **Description**                                                                                  |
|----------------|--------------------------------------------------------------------------------------------------|
| **Raw**        | Stores the ingested raw data.                                                                    |
| **Refined**    | Adds a `Processed` column to indicate successful processing.                                      |
| **Curated**    | Reverses values in the `FirstName` column (if it exists).                                         |
| **Enriched**   | Adds a `Bonus` column calculated as 10% of the `Salary` column (if it exists).                   |
| **Transformed**| Groups data by the `Category` column and sums up values in the `Value` column (if both exist).    |

---

## Instructions

### Prerequisites

- Python 3.8 or higher
- Install required dependencies using:
  ```bash
  pip install -r requirements.txt

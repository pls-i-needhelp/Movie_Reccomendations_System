# Movie Recommendation System

## Overview
This project implements a **Movie Recommendation System** using **content-based filtering**. The system recommends movies similar to the one selected by the user by analyzing movie features and calculating similarity scores. It uses **cosine similarity** to measure how close two movies are based on their content attributes such as genres, keywords, cast, and crew.

## Features
- Content-based movie recommendations  
- Utilizes movie metadata for similarity computation  
- Data preprocessing and feature extraction from datasets  
- Cosine similarity-based recommendation engine  
- Simple and interactive interface for querying movies  

## Dataset
The dataset used in this project is derived from **TMDB (The Movie Database)**.  
It contains metadata of movies, including:
- Title  
- Overview (plot summary)  
- Genres  
- Cast and crew details  
- Keywords  

These columns are preprocessed and combined to create a feature vector for each movie.

## Workflow
1. **Importing Dependencies**  
   Load essential Python libraries such as `pandas`, `numpy`, and `scikit-learn`.

2. **Data Collection and Pre-processing**  
   Load datasets, merge relevant columns, clean missing values, and remove duplicates.

3. **Feature Extraction**  
   Combine text features (genres, keywords, cast, crew, and overview) into a single column called `tags`.

4. **Text Vectorization**  
   Convert the textual data into numerical vectors using `CountVectorizer` from scikit-learn.

5. **Similarity Calculation**  
   Compute pairwise **cosine similarity** between movie vectors to quantify how similar they are.

6. **Recommendation Function**  
   Implement a function that takes a movie name as input and outputs the top similar movies based on cosine similarity.

## Technologies Used
- Python 3.x  
- Jupyter Notebook  
- Pandas  
- NumPy  
- scikit-learn  

## Results
The model successfully recommends movies with similar genres, cast, and storyline.  
For example, if you input *Inception*, the system might recommend *Interstellar*, *The Matrix*, or *Shutter Island* due to their shared themes and style.

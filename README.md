# Personalized Book Recommender

## Project Overview
The **Personalized Book Recommender** is a web application that recommends books based on user preferences. Leveraging the **Book-Crossing dataset** from Kaggle, this system utilizes **cosine similarity** for recommendations and **pandas** for data analysis. The model is built with **Python** and preserved using the **pickle** library for persistence. The web application is built using **Streamlit**, allowing users to input book details and receive personalized suggestions.

## Features
- **User-Friendly Interface**: A simple interface built using **Streamlit**, where users can input book preferences and receive recommendations.
- **Cosine Similarity**: A recommendation engine that finds similar books based on user preferences.
- **Persistent Model**: The model is saved using **pickle** to allow quick reloading without retraining.
- **Data-Driven**: Uses the **Book-Crossing** dataset from Kaggle to power the recommendation system.

## Dataset
The **Book-Crossing dataset** consists of three main files: **Users**, **Books**, and **Ratings**.

### 1. Users
This file contains anonymized user data, including their location and age (if available).

- **User-ID**: Anonymized identifier for the user.
- **Location**: Location of the user.
- **Age**: Age of the user (may contain NULL values).

### 2. Books
Books are identified by their ISBN, with additional metadata such as title, author, year of publication, and publisher. URLs for cover images are also provided.

- **ISBN**: Unique identifier for each book.
- **Book-Title**: Title of the book.
- **Book-Author**: Author of the book.
- **Year-Of-Publication**: Year the book was published.
- **Publisher**: The publisher of the book.
- **Image-URL-S**: URL for the book cover in small size.
- **Image-URL-M**: URL for the book cover in medium size.
- **Image-URL-L**: URL for the book cover in large size.

### 3. Ratings
This file contains user-submitted ratings for books, either as explicit ratings (on a scale from 1-10) or implicit ratings (marked as 0).

- **User-ID**: Identifier of the user who rated the book.
- **ISBN**: Unique identifier of the book that was rated.
- **Book-Rating**: Rating given by the user, where 0 represents implicit feedback, and 1-10 represents explicit ratings.



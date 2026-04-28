# Task 3: Exploratory Data Analysis (EDA) - Netflix Dataset

## Problem Statement
The objective of this task is to perform Exploratory Data Analysis (EDA) on the Netflix dataset to identify important trends, patterns, and insights related to the content available on Netflix. The analysis focuses on understanding the structure of the dataset, cleaning the data, and visualizing key relationships.

## Dataset Details
- **Dataset Name:** Netflix Titles Dataset
- **Source:** Kaggle / Public Netflix dataset
- **File Used:** `netflix_titles.csv`

### Dataset Features
The dataset contains information about Netflix content, including:
- `show_id` - Unique ID of the content
- `type` - Type of content (`Movie` or `TV Show`)
- `title` - Title of the content
- `director` - Director name
- `cast` - Cast members
- `country` - Country of production
- `date_added` - Date when content was added to Netflix
- `release_year` - Original release year
- `rating` - Age rating
- `duration` - Duration in minutes or number of seasons
- `listed_in` - Genre/category
- `description` - Short summary of the content

## Approach

### 1. Data Loading
- Imported the dataset using `pandas`
- Examined dataset shape, columns, and data types

### 2. Data Cleaning
- Checked for missing values
- Removed duplicate records
- Converted `date_added` into datetime format
- Filled missing values in important columns such as `director`, `country`, `cast`, `rating`, and `duration`
- Extracted additional columns like:
  - `year_added`
  - `month_added`
  - `duration_min` for movies

### 3. Exploratory Data Analysis
Performed analysis to answer questions such as:
- What is the distribution of Movies vs TV Shows?
- Which countries contribute the most content?
- How has Netflix content addition changed over the years?
- What are the most common genres?
- What are the most frequent content ratings?
- What is the duration distribution of movies?

### 4. Visualization
Used `matplotlib` and `seaborn` to create visualizations such as:
- Count plot of content type
- Bar chart of top countries
- Line chart of yearly additions
- Bar chart of top genres
- Rating distribution plot
- Histogram of movie durations


## Results
The EDA revealed several useful insights:

- Movies are more common on Netflix than TV Shows
- A few countries contribute the majority of Netflix content
- Netflix content additions increased significantly over recent years
- Some genres are much more dominant than others
- Mature audience ratings appear frequently in the dataset
- Most movies fall within a common runtime range

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn


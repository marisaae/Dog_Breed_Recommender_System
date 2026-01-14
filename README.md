# Dog Breed Recommender System

## Overview
The Dog Breed Recommender System is an unsupervised machine learning application designed to help potential dog adopters select breeds that best align with their preferred traits. By matching users’ selected characteristics to breed profiles, the tool improves adoption satisfaction, reduces return rates, and helps shelter staff manage resources more effectively.

## Key Features
- Interactive dashboard allowing users to select desired dog traits and receive top breed recommendations
- Data visualizations highlighting breed characteristics, common traits, and trait co-occurrence patterns
- Machine learning recommendation engine using cosine similarity to rank breeds based on similarity to user-selected traits
- Reusable data processing pipeline that cleans, encodes, and transforms breed data for both visualization and modeling

## Data Sources
- Open-source dataset of over 100 dog breeds from Kaggle, including traits such as size, lifespan, temperament, fur colors, and common health characteristics
- Data preprocessed in Python using pandas, including deduplication, trait standardization, one-hot encoding, and integration into an analysis-ready format

## Tech Stack
- **Languages:** Python  
- **Libraries & Tools:** pandas, scikit-learn, Plotly, Voila  
- **Deployment:** Jupyter Notebook

## Analysis & Modeling
Breed and trait data were cleaned, normalized, and structured to support both visualization and recommendation. Each breed was represented as a binary feature vector for its traits, and user-selected traits were compared using cosine similarity to identify the top matching breeds. The model’s performance was validated with clustering and silhouette analysis (score ≈ 0.6967), demonstrating meaningful grouping of breeds with similar characteristics. Visualizations provide additional insights into trait distributions, co-occurrence, and breed profiles.

## Visualizations & Insights
- Top breed traits overall and by size category
- Heatmap showing co-occurrence of traits across breeds
- Interactive dashboard allowing users to explore breed characteristics by hovering over charts

## User Guide
1. Download and extract the project ZIP folder containing `dog_breeds.csv`, `app.ipynb`, and `requirements.txt`.  
2. Open the folder in your preferred IDE.  
3. Install dependencies: ```pip install -r requirements.txt```
4. Launch the application: ```voila app.ipynb```
5. In the dashboard, scroll to the trait selection checkboxes, select at least one character trait, and click Submit to view recommended breeds.

## Future Improvements
- Enhance visualizations for more interactive comparison of breeds
- Explore alternative recommendation algorithms and ranking methods
- Expand data sources to include detailed other breed characteristics and environmental factors for a more precise and personalized recommendation system


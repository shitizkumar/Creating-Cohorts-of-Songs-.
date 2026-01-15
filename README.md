 Song Cohort Discovery using Exploratory Data Analysis & Unsupervised Learning
Executive Summary

This project applies exploratory data analysis (EDA) and unsupervised machine learning to segment songs into distinct cohorts based on audio and popularity features. The objective is to uncover latent patterns in music data that can support recommendation systems, playlist curation, and user behavior analysis.

The project emphasizes analytical reasoning, feature understanding, and interpretability rather than treating clustering as a black-box technique.

Business Context & Motivation

Music platforms rely heavily on accurate content segmentation to:

Personalize user recommendations

Generate mood-based and activity-based playlists

Improve user engagement and retention

By grouping songs into cohorts with similar characteristics, stakeholders can better understand what drives similarity between songs and how these groupings can be leveraged in downstream applications.

Problem Definition

Given a dataset of songs with multiple numerical features, the goals are to:

Perform in-depth EDA to understand feature distributions and relationships

Identify key variables influencing song similarity

Segment songs into meaningful cohorts using clustering algorithms

Interpret and validate the resulting clusters

Dataset Description

The dataset consists of song-level numerical attributes, including:

Audio features (e.g., tempo, energy, danceability)

Popularity-related metrics

Other continuous variables relevant to musical characterization

Prior to modeling, data quality checks and preprocessing steps were applied to ensure reliable analysis.

Technical Stack

Python – primary programming language

Pandas – data manipulation, aggregation, and groupby()-based analysis

NumPy – numerical computations

Matplotlib & Seaborn – statistical visualization and EDA

Scikit-learn – feature scaling and clustering (K-Means)

Methodology
1. Data Exploration & EDA

Analyzed feature distributions, variance, and correlations

Used groupby() operations to compare song characteristics across different segments

Visual insights from EDA guided feature selection and modeling decisions

2. Feature Engineering & Preprocessing

Selected relevant numerical features for clustering

Applied standardization to ensure distance-based models are not biased by feature scale

3. Clustering Approach

Implemented K-Means clustering to identify latent song cohorts

Determined an appropriate number of clusters based on exploratory analysis

Assigned cluster labels for downstream interpretation

4. Cluster Interpretation

Examined feature profiles within each cluster

Identified distinct musical patterns and cohort characteristics

Linked technical results to real-world music analytics use cases

Key Findings

Songs form distinct cohorts driven by combinations of tempo, energy, and popularity

Each cluster represents a unique musical profile rather than arbitrary segmentation

Unsupervised learning effectively reveals hidden structure in high-dimensional music data

Reproducibility

To run this project locally:

git clone https://github.com/shitizkumar/Creating-Cohorts-of-Songs-..git


Install dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn


Open the notebook:

song_cohart.ipynb

Limitations

Clustering performance is sensitive to feature selection and scaling

K-Means assumes spherical clusters and may not capture complex structures

Results are exploratory and should be validated before production use

Future Enhancements

Compare K-Means with DBSCAN and Hierarchical Clustering

Introduce cluster evaluation metrics (Silhouette Score, Davies–Bouldin Index)

Integrate the cohorts into a recommendation or playlist generation pipeline

Build an interactive visualization/dashboard for business stakeholders

Conclusion

This project demonstrates a structured, analytical approach to unsupervised learning problems. It highlights the importance of EDA, feature understanding, and interpretability when applying clustering techniques to real-world datasets.

Author

Shitiz Choudhary
Aspiring Data Scientist | Machine Learning | Analytics

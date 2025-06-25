1. Description
   
    Hackathon Problem Statement: NDVI-based Land Cover Classification

3. Key Concepts

    NDVI (Normalized Difference Vegetation Index) = (NIR - RED) / (NIR + RED)
   
    vegetation health using satellite data:
   
    Where:-
   
     NIR = Near-Infrared reflectance
   
     Red = Red reflectance
   
5. Data Challenges
   
    Noise: The main challenge with the dataset is that both the imagery and the crowdsourced data contain noise (due to cloud cover in the images and inaccurate labeling/digitizing of polygons).

    Missing Data: Certain NDVI values are missing because of cloud cover obstructing the satellite view.

    Temporal Variations: NDVI values vary seasonally, requiring careful feature engineering to extract meaningful trends.

7. Important Note:
   
    The training and public leaderboard test data may contain noisy observations, while the private leaderboard data is clean and free of noise.
    This design helps evaluate how well your model generalizes beyond noisy training conditions.

9. Dataset
    
    Each row in the dataset contains:

     class: Ground truth label of the land cover type — one of {Water, Impervious, Farm, Forest, Grass, Orchard}

     ID:Unique identifier for the sample

     27 NDVI Time Points: Columns labeled in the format YYYYMMDD_N (e.g., 20150720_N, 20150602_N) represent NDVI values collected on different dates.
     These values form a time series representing vegetation dynamics for each location.

11. Rules
    
     Model: Logistic Regression only (multiclass).

     Preprocessing: Denoising, imputation, and feature engineering allowed.

7. Leaderboard:

    Public (89% test data): Immediate feedback.

    Private (11% test data): Final ranking (avoids overfitting).

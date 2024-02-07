# MusicRecommendation
Spotify Playlist Recommendation using Matrix Completion with Alternating Minimization.
implementation of the theoretical work of (Hardt, 2014) https://arxiv.org/abs/1312.0925.

This project seeks to implement matrix completion for an artist recommendation algorithm for specific users?
Playlist download tool for Spotify: Exportify
https://exportify.net/

## Motivation
- How do recommendation algorithms work, e.g. Spotify and Netflix?
- What new artists should be recommended for users, given we have a general sense of their music taste? 
- Which users have the most similar music taste, considering what artists were recommended to them? 

## Normalization
Normalized values by row to find recommendations for each user ensure that each recommendation value was on a consistent scale.
- Top artist for each user has been scaled such that the max value is 1.0
- Artist that has the value of 1.0 is the artist that shows up the most in their playlists


# Model Fit & Convergence
Notably, we used a small dataset of only:
- 2808 artists
- 125 playlists 

Which resulted in the optimal parameters of k = 58 and T =  ~200 for playlist dataset, and k = 10 and T = ~10 for the user dataset.

<img width="660" alt="Screenshot 2024-02-07 at 10 18 56 AM" src="https://github.com/rhea-mal/MusicRecommendation/assets/70975260/6836b64c-6a5f-4fb6-9bf6-6ad630abf37e">


# Analysis & Visualization
<img width="673" alt="Screenshot 2024-02-07 at 10 21 27 AM" src="https://github.com/rhea-mal/MusicRecommendation/assets/70975260/2f1ea3cc-25d5-4d4a-bce1-6899a716c2ea">

PCA of user preferences by Euclidean Distance 

<img width="600" alt="Screenshot 2024-02-07 at 10 19 55 AM" src="https://github.com/rhea-mal/MusicRecommendation/assets/70975260/fdb73910-7ea3-4c33-a240-430947c1bda8">
<img width="658" alt="Screenshot 2024-02-07 at 10 23 32 AM" src="https://github.com/rhea-mal/MusicRecommendation/assets/70975260/c88742eb-a4a7-4f75-ac20-66f9e67ba1fe">

<img width="272" alt="Screenshot 2024-02-07 at 10 19 37 AM" src="https://github.com/rhea-mal/MusicRecommendation/assets/70975260/848c5933-e813-4ea9-a7d0-c09e7bcf6d94">

Genre Analysis Post-hoc:

<img width="274" alt="Screenshot 2024-02-07 at 10 20 36 AM" src="https://github.com/rhea-mal/MusicRecommendation/assets/70975260/6b3217a6-e1a6-4695-ab11-5a4614d43d99">

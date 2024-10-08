### Movie Recommendation Engine

This repo contains a movie recommendation system using a combination of Graph Neural Network (GNN) layers (specifically GCN and GAT) integrated with a Factorization Machine (FM). The main goal is to predict unknown user-item interactions in a bipartite graph of users, items as nodes and ratings as edges.

The movielens dataset is split into train and test sets based on the timestamp of interactions for better results. An adjacency matrix is created to represent the interactions for use in GNN layers. A `GNNLayer` combines GCN and GAT layers to learn rich embeddings for users and items. Factorization Machine Model integrates these embeddings to predict interactions and the model is trained and evaluated using ranking metrics like HitRatio (HR) and Normalized Discounted Cumulative Gain (NDCG)

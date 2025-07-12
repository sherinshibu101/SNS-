#Influence Minimization in Social Networks via GNNs
Problem Addressed
This project tackles the challenge of limiting the spread of misinformation and harmful content in large-scale social networks. By modeling the network as a unified, heterogeneous directed graph with semantic edge weights, the goal is to identify and suppress the most influential nodes, thereby reducing the potential for widespread information cascades.

Approach
Unified Graph Construction: All user interactions (follows, retweets, replies, mentions) are merged into a single directed multigraph, preserving both structural and semantic information.

Node Feature Engineering: Each user is described by a 14-dimensional feature vector capturing behavioral and topological attributes.

Influence Labeling: Influence scores are assigned to nodes using time-aware cascade simulations to reflect realistic diffusion dynamics.

Modeling: Multiple GNN architectures (GCN, GraphSAGE, Graphormer) are trained independently to predict node influence.

Intervention Evaluation: The top 30% most influential nodes (per model) are removed, and the resulting reduction in simulated information spread is measured using the Independent Cascade Model.

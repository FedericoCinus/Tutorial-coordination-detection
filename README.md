# Coordination Detection via Similarity Graph

This repository provides a pipeline for detecting coordinated behavior between users based on shared URLs. Starting with raw user-URL data, it computes pairwise similarities, constructs a graph, and visualizes coordinated groups interactively.

## Features
- **Data Aggregation**: Groups URLs shared by each user for efficient similarity computation.
- **Similarity Calculation**: Uses TF-IDF and cosine similarity to build a sparse similarity matrix, optimized for GPU if available.
- **Graph Construction and Filtering**: Builds a NetworkX graph with customizable filters for similarity score and shared URLs.
- **Interactive Visualization**: Visualizes the coordination network with PyViz, including clickable profile links for each user.


## Setup

**Clone the Repository**
   ```bash
   git clone https://github.com/your-username/coordination-detection-visualization.git
   cd coordination-detection-visualization
   ```



## Usage

1. **Data Preparation**: Aggregate URLs by user, then calculate similarity using TF-IDF and cosine similarity.
2. **Graph Construction**: Build a graph from the similarity matrix, filtering edges by similarity score and shared URL count.
3. **Visualization**: Use PyViz to render the graph interactively, with optional clickable profile links for each user.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

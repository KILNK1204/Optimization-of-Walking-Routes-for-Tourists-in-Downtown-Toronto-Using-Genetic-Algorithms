# Optimization of Walking Routes for Tourists in Downtown Toronto

This project presents a hybrid algorithm that optimizes walking routes for tourists visiting downtown Toronto. By combining Genetic Algorithms (GA) with Depth-First Search (DFS), the model generates scenic and efficient walking paths that start and end at a user-defined location.

## Project Objective

To help tourists plan the most enjoyable walking route that:
- Covers major points of interest (POIs)
- Minimizes walking distance
- Maximizes scenic appeal
- Returns to the starting point

## Key Features

- **Hybrid GA Algorithm**: GA explores optimal route combinations.
- **Custom Fitness Function**: Balances travel distance and scenic score using weighted parameters.
- **Scenic Score Modeling**: Streets are scored based on nearby attractions using Google Places and OSM data.
- **Graph-Based Modeling**: The city is modeled as a graph (nodes = intersections, edges = roads with scenic and distance weights).
- **Dynamic Virtual Nodes**: Handles POIs located mid-road using virtual split points in the graph.

## Data Sources

- **Google Places API**: Tourist attraction metadata and ratings.
- **OpenStreetMap (OSM)**: Street network and spatial structure of downtown Toronto.
- **OSMnx**: Used for street graph extraction and processing.

## Visualizations

- **Scenic Heatmap** of downtown POIs.
- **Color-coded Street Network** based on scenic scores.
- **Final Optimized Route** shown over Toronto’s street map.

## Optimization Goals

Minimize:
Where `λ` is a weight factor that balances route efficiency and attraction appeal.

## Performance

- Fast convergence of GA within 30 iterations
- Robust route quality across multiple runs
- Tested using Google Colab with GPU acceleration

- ## Authors

- **Zhaoheng Li** 
- **Songyuan Sang** 

## Related Medium Article

🔗 [Read our write-up on Medium](https://medium.com/ai4sm/optimization-of-walking-routes-for-tourists-in-downtown-toronto-88407ce38c75)

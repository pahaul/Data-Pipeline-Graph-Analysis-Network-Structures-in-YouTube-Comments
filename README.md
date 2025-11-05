# Data-Pipeline-Graph-Analysis-Network-Structures-in-YouTube-Comments
This project implements an ETL pipeline in Python to aggregate, clean, and model unstructured data originating from the comment sections of several thematically similar YouTube videos. The goal is to create a network structure (Graph Data Modeling) to visualize the interactions and overlaps of the Top 50 commentators across various video channels.

---

While the original goal was to find linguistic correlations in comments, the following key challenges were solved from a Data Engineering perspective:

Data Ingestion: Processing of heterogeneous CSV files (sourced via the YouTube Data Tools API) from multiple sources (6 different YouTube videos/channels).

Data Transformation (ETL): Consolidation of the distinct comment datasets into one central, cleaned Pandas DataFrame.

Data Modeling: Reduction and filtering of the dataset to identify the Top 50 commentators and subsequent creation of a Pivot Table to quantify interactions, which serves as the foundation for the network edges.

Relationship Visualization: Utilizing Python libraries to map complex relations (commentator comments on video, commentator replies to commentator) into an interactive network diagram.

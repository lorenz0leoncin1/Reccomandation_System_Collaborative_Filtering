# Big Data Project

## Collaborative Filtering

**Core Idea:** Collaborative filtering predicts an actor’s preferences based on the preferences of similar actors.

**Implementation:**
- **Similarity Matrix:** We calculated actor similarities based on the movies they've worked in and the genres of those movies.
- **Recommendations:** We recommended movies to an actor based on what similar actors have done, filtered through genres that the target actor frequently works in.

## Content-Based Filtering

**Core Idea:** Content-based filtering recommends items based on the features of the items and the preferences of the user.

**Implementation:**
- **Genres:** We incorporated movie genres to filter recommendations. This allows us to tailor the recommendations based on the genres that the actor has historically worked in, adding a layer of personalization.

## How Collaborative Filtering is Used

- **Utility Matrix:** Created a utility matrix where rows represent actors and columns represent movie-genre combinations. This matrix helps in calculating how similar actors are to each other.
- **Cosine Similarity:** Used cosine similarity to measure the similarity between actors based on the utility matrix. This step is a fundamental aspect of collaborative filtering.

## How Content-Based Filtering is Used

- **Genre Preference:** The recommendation process considers the genres that an actor has worked in most frequently. This adds a content-based element to the recommendations, as it ensures that the recommended movies align with the actor’s genre preferences.

## Summary

While the primary mechanism is collaborative filtering (using the similarity of actors based on their movie roles), the system also integrates content-based elements by considering movie genres. This hybrid approach enhances the quality of recommendations by combining the strengths of both methods:

- **Collaborative Filtering:** Identifies similarities between actors and suggests movies based on those similarities.
- **Content-Based Filtering:** Refines the recommendations by focusing on genres that match the target actor’s historical preferences.

This hybrid approach is often more effective than using collaborative or content-based filtering alone, as it leverages the benefits of both methodologies.


## Repository Structure
- `project_notebook.ipynb`: Main notebook.
- `docs/`: Documentation, including the LaTeX report.

## Notebook Execution
[![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-blue)](https://colab.research.google.com/drive/19tGUklqUuRvuhtNEyWCIR5LAqX5c5Ims#scrollTo=q-3e10StPCAL)


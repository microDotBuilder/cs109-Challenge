# Wildfire Risk Prediction with a Bayesian Network

This project focuses on predicting the risk of a wildfire starting or becoming large in a specific area, given certain conditions. The emphasis is on risk prediction rather than simulating fire spread.

## Core Idea

Develop a Bayesian Network to model the causal relationships between factors contributing to wildfire risk. A Bayesian Network is a directed acyclic graph where nodes represent random variables and edges denote conditional dependencies.

## Probability Modeling

- **Nodes:** Potential variables include Temperature, Humidity, Wind Speed, Human Activity (e.g., proximity to campsites or roads), Lightning Strike, and the final node, Fire Occurs.
- **Conditional Probability Tables (CPTs):** Each node is associated with a probability distribution conditioned on its parent nodes. For example, the probability of "Fire Occurs" is significantly higher if "Lightning Strike" is true and "Humidity" is low. These probabilities can be informed by research, expert intuition, or learned from historical data when available.

## Academic Sophistication

This project leverages key concepts from CS109, including conditional independence, the chain rule for Bayesian networks, and probabilistic inference. For instance, you can compute probabilities such as P(Fire Occurs | Temperature = High, Humidity = Low).

## Data for British Columbia (B.C.)

Historical weather and wildfire data for B.C. can be utilized to inform the CPTs. Complex machine learning is not required; instead, data analysis can help estimate conditional probabilities, such as examining weather conditions on days when large fires started.

## Implementation

Python libraries such as `pgmpy` can be used to construct and query the Bayesian Network.

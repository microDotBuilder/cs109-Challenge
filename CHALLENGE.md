## Idea : Wildfire Risk Prediction with a Bayesian Network

This idea is less about simulating the spread and more about predicting the risk of a fire starting or becoming large in a specific area, given certain conditions.

# The Core Idea:

Create a Bayesian Network that models the causal relationships between factors that contribute to wildfire risk. A Bayesian Network is a directed acyclic graph where nodes are random variables and edges represent conditional dependencies.

# The Probability:

[ ] Nodes: Your nodes could include variables like Temperature, Humidity, Wind Speed, Human Activity (e.g., near a campsite or road), Lightning Strike, and the final node Fire Occurs.
[ ] Conditional Probability Tables (CPTs): For each node, you would define a probability distribution conditioned on its parents. For example, the probability of a Fire Occurs would be very high if Lightning Strike is true and Humidity is low. You can define these probabilities based on research, intuition, or even by "learning" them from historical data if you can find a suitable dataset.

# Academic Sophistication:

This project directly uses one of the most powerful concepts from CS109. You can demonstrate your understanding of conditional independence, the chain rule for Bayesian networks, and how to perform inference (i.e., calculate the probability of one node given evidence about others). For example, you could calculate P(Fire Occurs | Temperature=High, Humidity=Low).

# Data for B.C.:

You can find historical weather data and fire data for B.C. You wouldn't need to do complex machine learning; instead, you could use the data to inform the probabilities in your CPTs. For example, you could look at the weather conditions on days when large fires started to estimate your conditional probabilities.

# Implementation: You can use Python libraries like pgmpy to build and run queries on your Bayesian Network.

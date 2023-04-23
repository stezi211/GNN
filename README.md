# GNN
GNN &amp; DBpedia

This notebook demonstrates how to perform the link prediction task on the Dbpedia graph dataset. The goal is to predict connections between scientists in the Dbpedia knowledge graph. To do this, the task is divided into two steps:
data collection and preprocessing, where data is collected from Dbpedia using SPARQL and cleaned and visualized before creating the final graph, and
prediction, where a Graph Neural Network called GraphSAGE is used to predict the probability of two nodes being connected on the existing network.
In order to use GraphSAGE, each node in the graph of scientists must have features that describe the corresponding scientist, such as their academic disciplines. Therefore, a second query is needed to obtain a dataframe of these features and align them with the corresponding nodes. As the graph includes labeled nodes, the link prediction task is treated as a supervised problem.

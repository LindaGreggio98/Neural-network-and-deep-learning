# Graph Neural Network for Node Classification

Node classification is a fundamental task in **graph-related machine learning**.  

Given a graph where each node belongs to one of k classes and has a **feature vector**, the goal is to predict the **class of each node**.  

- In **traditional machine learning**, only the feature vector is used for classification.  
- In **modern approaches**, the **graph topology** is leveraged to improve prediction accuracy.  

This project explores this evolution, gradually incorporating topological information: from **handcrafted topological features** to **node embeddings** and finally to **end-to-end graph neural networks (GNNs)**.  

Our experiments replicate central results from the literature and demonstrate **progression from classical methods to state-of-the-art techniques**.

All implementations are available at: [https://github.com/nicolopenzo/exploiting_graph_topology_for_node_classification](https://github.com/nicolopenzo/exploiting_graph_topology_for_node_classification). Here you can find the notebook on GNNs.

---

## Techniques

The following methods were implemented and compared:

1. **Topological Features + Classifier**  
   - Extract topological information from the graph (e.g., node degree, centrality).  
   - Combine it with the intrinsic node features.  
   - Train a traditional classifier to predict node labels.

2. **Node Embeddings + Classifier**  
   - Generate embeddings using a well-known technique such as **node2vec**.  
   - Feed the embeddings to a classifier to predict the node classes.  

3. **Graph Neural Networks (GNNs)**  
   - Use an **end-to-end trainable neural network** that directly leverages the graph structure and node features.  
   - The network predicts node labels without handcrafted features.

---

## Experiments

- Gradually incorporate **topological information** into the classification task.  
- Compare **traditional ML methods**, **embedding-based methods**, and **GNNs**.  
- Visualize the performance improvement as the model incorporates more structural information.  

---

## Key Takeaways

- Incorporating **graph topology** improves node classification performance.  
- Node embeddings provide richer representations than handcrafted topological features.  
- Graph neural networks allow **end-to-end learning** and achieve the best performance in most cases.



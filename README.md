# GNN_QNN_blocks_resistant_malaria

In this implementation, each individual molecule is treated as a distinct graph where atoms act as nodes and chemical bonds serve as edges. By structuring the data this way, the GNN learns an "internal language" of the molecule based directly on its structural connectivity rather than external similarity metrics. This approach, often referred to as Molecular Property Prediction, allows the model to leverage structural intelligence, such as distinguishing between linear chains and ring systems, which is vital for understanding biological interactions.

As information flows through the network, the GCNConv layers aggregate features from neighboring atoms, ensuring that a Carbon atom's representation is uniquely informed by its specific local environment (e.g., whether it is bonded to Oxygen versus Hydrogen). This process, known as message passing, enables the model to generalise across the chemical space by identifying common functional groups and structural motifs.

Through these sequential passes, the model builds a sophisticated, hierarchical understanding of the molecule’s chemical identity, starting from local atomic interactions and scaling up to global molecular properties.

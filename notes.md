# Incorporating symbolic knowledge in Knowledge Graph Embeddings

Motivation / introduction:
- many ways of embedding a knowledge graph
- excellent at learning representations of the dataset
- often with KGs we can provide other knowledge as well
- a priori statements about all of the dataset, or certain parts of it
    - 'all edges in the dataset are transitive'
    - 'for all people, the ancestor of my ancestor is also my ancestor'
- we would like our training to benefit from such knowledge
- this is hard because we want to keep the efficiency of KGE, but also add
    richer knowledge, but only in training the model.

Background:
- pt 1: KG
- how is a KG defined?
- ways of training a KG
    - modelling
    - typical loss
    - open / closed world hypothesis
        - importance of symbolic knowledge in offsetting open world

- pt 2: first order sentences
- brief about PDBs
- TractOR
    - tractor's connection to PDBs
    - what tractor solves with PDB querying

Our method:
- why we want to build upon tractor
- what TractOR cannot solve wrt PDBs
- a simple solution to overcoming this
- some reasoning as to why this could work

Experiments:
- describe the experiment setup
- obviously no output yet

Other work / future work:
- extending this to models with not obvious predicates
    - cf propositional logic semantic loss of softmax output

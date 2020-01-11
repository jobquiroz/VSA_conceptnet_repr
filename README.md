# VSA_conceptnet_repr

Concept representation model using Vector Symbolic Architectures

## Description.

This repository includes all the files developed for the (under review) paper "Semantic Similarity Estimation using Vector Symbolic Architectures".

Vector Symbolic Architectures are a family of methods that use high-dimensional vectors to represent objects: concepts, trees, sequences, etc. In this work we selected a binary VSA called Binary Spatter Codes proposed by Pentti Kanerva. Based on this VSA we designed a model for concept representation that creates "Semantic Pointers" based on a set of semantic features.

We took the idea of semantic pointers from Eliasmith's model Semantic Pointer Architecture. Semantic pointers are vectors used to point to information within a memory system, therefore the term pointer. However, semantic pointers are also 'semantic', which means that the pointers themselves are similar to the information they reference.

We create these semantic pointer based on a set of semantic features, which are words that try to define a concept based on its relations with other words. We obtain the semantic features from the [ConceptNet] (http://conceptnet.io/) knowledge base. In this experiments we use the SimLex-999 dataset to represents its concepts and then compare how our similarity estimation between pairs is approximate to the ranks assigned. 

## File Description

The repository contains two folders: Code and Data. Within Code there are three notebooks: VSA-Experiments, EncodingDataset and HDComputing_basics.

### Notebooks (/Code)
Description of files. All codes were implemented as Python Notebooks.

#### 1) HDComputing_basics
This is an implementation of a Vector Symbolic Architecture (VSA) for a semantic net exploration.
In this notebook a class of objects for hyperdimensional vectors is implemented. It's most important built-int functions are the initialization and the arithmetical operations: addition, multiplication and permutation. It is also described functions for creating, storing and retrieving vectors from memory. 

#### 2) HDComputing_Tests
This notebook makes several experiments using the arithmetic operations defined in the previous notebook. For anyone trying to start learning about operations and the properties of high-dimensional spaces. This is the place to go.

#### 3) Collecting_features.
This notebook shows the basic functions used to request information from the ConceptNet Web API, and then organizing such information as semantic features of the SimLex-999 dataset. 

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

### Authors
Job Isaias Quiroz Mercado. PhD Student at Centro de Investigación en Computación - Instituto Politécnico Nacional - México

### License
[MIT](https://choosealicense.com/licenses/mit/)

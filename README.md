**Molecular-property-prediction**
This project implements machine learning models to predict solubility from chemical structures.

**Project overview**
workflow of the project is as follows
- Process molecular data from the ESOL dataset
- Extract chemical features from molecular structures.
- Train traditional ML models (Random Forest)
- Implement Graph Neural Networks for molecular property-(solubility) prediction 
- Compare and evaluate model performance

**Repository Structure**
molecular_property_prediction/
├── data/
│   ├── raw/
│   │   └── delaney-processed.csv          # Original ESOL dataset
│   └── processed/
│       └── processed_esol_data.csv        # Processed dataset with molecular features
├── notebooks/
│   ├── 01_data_acquisition.ipynb          # Data download and initial processing
│   ├── 02_basic_model.ipynb               # Random Forest implementation
│   ├── 03_graph_neural_network.ipynb      # GNN model implementation
│   └── 04_model_comparison.ipynb          # Comparison of model performance
├── src/
│   ├── data_processing/
│   │   ├── __init__.py
│   │   ├── molecular_features.py          # Feature extraction functions
│   │   └── graph_conversion.py            # Molecule to graph conversion
│   ├── models/
│   │   ├── __init__.py
│   │   ├── random_forest.py               # Random Forest model implementation
│   │   └── gnn_model.py                   # Graph Neural Network implementation
│   └── visualization/
│       ├── __init__.py
│       └── visualization.py               # Plotting and visualization functions
├── results/
│   ├── figures/
│   │   ├── model_comparison.png           # Performance comparison visualization
│   │   ├── feature_importance.png         # Random Forest feature importance
│   │   ├── molecule_visualization.png     # Molecule visualization with atom contributions
│   │   ├── rf_predictions.png             # Random Forest predictions plot
│   │   └── gnn_predictions.png            # GNN predictions plot
│   └── models/
│       ├── random_forest_model.pkl        # Saved Random Forest model
│       └── gnn_model.pt                   # Saved GNN model
├── environment.yml                        # Conda environment specification
├── requirements.txt                       # Python package requirements
└── README.md                              # This file

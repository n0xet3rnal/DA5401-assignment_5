# DA5401 Assignment 5 - Notebook Summary

## File Structure
```
├── assn5.ipynb # Main analysis notebook
├── README.md   # This file
└── data
    ├── yeast.arff # Dataset used for analysis
    └── yeast.xml # Dataset used for analysis
```

## Notebook Structure
### Imports
- Import all required Python libraries.

### Loading Data
- Load the yeast dataset and extract features and labels.

### Preprocessing
- Analyze label patterns, select categories, and standardize features.

### Dimensionality Reduction & Visualization
- Apply t-SNE and Isomap to visualize data structure and category separability.

### Analysis of Data Veracity
- Interpret visualizations to discuss noisy labels, outliers, and classification difficulty.

### Comparison and Curvature Analysis
- Compare Isomap and t-SNE, and relate data manifold complexity to classification.


## Input Data

The analysis is based on the **Yeast dataset**, a well-known benchmark in multi-label classification. The dataset consists of two key components:

1. **Feature Matrix (X)**  
   - Contains gene expression profiles represented by **103 continuous-valued features**.  
   - Each row corresponds to a yeast gene, and each column represents a specific gene expression measurement or derived feature.  

2. **Label Matrix (Y)**  
   - A **binary multi-label matrix** with **14 possible functional categories**.  
   - Each entry indicates whether a given gene is associated with a particular functional class.  
   - Since the dataset is multi-label, a single gene can belong to multiple functional categories simultaneously.  

### Source and Availability  
The Yeast dataset is widely available from machine learning repositories, including the [MULAN Repository](http://mulan.sourceforge.net/datasets.html).  
- The standard distribution provides the files in **ARFF format** (`yeast.arff` for features and the corresponding label file).  
- Pre-converted versions are also available in **CSV** or **NumPy** formats for direct use in machine learning pipelines.  

---  




## How to Use
1. Open `assn5.ipynb` for annotated analysis with results and plots.  
2. Ensure the dataset file is placed inside the `data` directory as shown above.  

## Requirements
- Python 3.x  
- pandas, numpy, scikit-learn, matplotlib, seaborn, scipy

Install dependencies with:  
```bash
pip install pandas numpy scikit-learn matplotlib seaborn scipy
```

## Author

*Jerry Jose (BE22B022)*  
*IITM Data Analytics Lab, Semester 7*
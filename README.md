# Read Me!
Classifying Cancerous Genetic Mutation Variations

## About
For this project, I used a variety of classification models to categorize the malignancy of genetic mutation variations based on data derived from the text of expertly annotated scientific literature. The ultimate ensemble classification model is based on exploration using Multinomial Naive Bayes, Logistic Regression, Linear SVMs, and Random Forests.

## Data
Data come from a [Kaggle Competition](https://www.kaggle.com/c/msk-redefining-cancer-treatment/data) sponsored by [Memorial Sloan Kettering Cancer Center](https://www.mskcc.org). Using the contest's nomenclature, *training data* include expert-defined class identification (i.e., Class 1-9), and *test data* (with no class identification) are used to to for scoring the competition. Therefore, I split the provided *training data* for training and testing my models.

- **Training Variants,** comma separated file containing information about the genetic mutations
   - **ID**, id number of the row used to link the mutation to the clinical evidence''
   - **Gene**, the gene where this genetic mutation is located
   - **Variation**, the amino acid change for this mutation
   - **Class**, the class this genetic mutation has been classified on (1-9; no descriptions are provided for class assignments)  
   
   
- **Training Text**, a double pipe (||) delimited file containing clinical evidence (text) used to classify genetic mutations
   - **ID**, id number of the row used to link the clinical evidence to the genetic mutation
   - **Text**, the clinical evidence (scientific literature) used to classify the genetic mutation

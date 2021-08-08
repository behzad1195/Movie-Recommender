# Movie Recommender
* Build a movie recommender website using 'MovieLens' Dataset
* Two recommender models has been used for providing the recommendations
    + 1. Collaborative Filtering With Non-negative Matrix Factorization (NMF)
    + 2. Item-based Collaborative Filtering (find similar movies instead of similar users) using CSR matrix and KNN with 'cosine similarity' as the method
* Contributors: [Francesco Mari](https://github.com/fra-mari) and [Laura Bertolini](https://github.com/Rellino)


## Repo Structure

### 1. Webapp
#### 1.1 models
* Stored version of KNN model -> [knn.pickle]()
* Stored version of NMF model -> [NMF_model.pickle]() and [NMF_R.pickle]()

#### 1.2 Static
* Website simple Design -> styles.css

#### 1.3 templates
* HTML files -> [knn_recommender.html](), [main_knn.html](), [main.html](), [recommender.html]()

#### 1.4 Models and Web application
* Website structure -> [app.py]()
* Collaborative Filtering model (NMF) > [recommending_engine.py]()
* Item-based Collaborative Filtering model (KNN) > [knn_recommending_engine.py]()

### 2. Data
* Raw data from MovieLens -> [links.csv](), [movies.csv](), [ratings.csv](), [tags.csv]()
* Info about the content of data -> [README.txt]()
* Final data after merge and imputation on missing values -> [df_final.csv]()

### 3. Files 
* MICE model (Multivariate Imputation by Chained Equations) for filling the missing value [MICE_imputer.py]()
* Environment specs -> [requirements.txt]() 
# Topic Modeling Disney Reviews 

-   Author: Amelia Tang 

## About
Disney land is regarded as "The Happiest Place on Earth" by many according to U.S. News Travel (Anonymous 2021). This Natural Language Processing (NLP) project is to visualize and analyze the Disneyland Reviews data set I collected from [Kaggle](https://www.kaggle.com/datasets/arushchillar/disneyland-reviews). The dataset comprises approximately 42,000 reviews of three Disneyland locations: Paris, California, and Hong Kong. To facilitate data visualization, I created a Tableau story that provides an overview of ratings by branches and reviewer locations. For text data preprocessing, I performed basic text cleaning (e.g., removing digits), as well as stemming and lemmatization. In the project, I utilized two methods, TextBlob and NLTK VADER, for sentiment polarity analysis and compared the polarity scores assigned by both methods.

<br>For topic modeling, I utilized Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN) and Latent Dirichlet Allocation (LDA) models to identify clusters/topics. However, the topics are hard to interpret as both models do not output semantic topics.  

<br>Finally, I used ChatGPT prompt engineering...

## Reports
EDA report (Pre-processing and sentiment analysis) can be found [here](https://github.com/aimee0317/topic_modeling_Disney_reviews/blob/main/EDA/Disney_EDA_Report.pdf).
<br>NLP modeling report (LDA and HDBSCAN) can be found [here](https://github.com/aimee0317/topic_modeling_Disney_reviews/blob/main/src/NLP_Model.pdf).

## Visualizations 

### Tableau 
![Tableau Demo](EDA/disney-tableau-demo.gif)

### WordCloud 
#### Unigram WordCloud
![Unigram WordCloud](EDA/wordcloud.png)

#### Bigram WordCloud
![Bigram WordCloud](EDA/bi_gram_wordcloud.png)

### HDBSCAN Clusters 
![HDBSCAN Clusters](src/HDBSCAN_cluster.png)


## Usage

### Creating the environment

At the project root
`conda env create --file topic_modeling_disney.yaml`

<br>Run the following command from the environment where you installed
JupyterLab.

`conda install nb_conda_kernels`

## Dependencies

[TBU]A complete list of dependencies is available [here](TBU).
<br>- Python 3.10.8 and Python packages: <br>- docopt=0.6.2 <br>-
altair=4.2.0 <br>- altair_data_server=0.4.1 <br>- scikit-learn=1.2.0 <br>- xgboost=1.7.1

## References 
Anonymous. 2021. “Disneyland Resort Reviews | U.S. News Travel.” "https://travel.usnews.com/Anaheim_Disneyland_CA/Things_To_Do/Disneyland_62335/".

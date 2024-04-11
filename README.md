# FashoReco: H&M Personalized Fashion Recommendations

Welcome to the **FashoReco** GitHub repository. This project was developed as part of the BT4222 module, with the aim to enhance H&M customer experiences through personalized product recommendations. By analyzing customer purchase history and transactional behaviors, our recommendation system provides targeted product suggestions, improving shopping efficiency and satisfaction.

## Contributors
- Dylan Lo
- Li Shuyao
- Nicholas Teow
- Alden Sio
- Bernice Saw
- Xu Wenxuan

## Technologies and Requirements

**Programming Language:** Python 3.8+

**Required Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, pickle, among others.

**Data:** Our system utilizes H&M's extensive datasets, including customer data, transactions data, and articles data. These datasets form the backbone of our analysis and can be found at the following Kaggle competition link: [H&M Personalized Fashion Recommendations](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/overview).

## Project Workflow

Our project is structured into a series of Jupyter notebooks, each covering a specific phase of the recommendation system development process. At every step, we generate pickle files for efficient data transfer and continuity between phases. Each notebook includes a detailed step-by-step guide, outlining our analytical process and the rationale behind our decisions.

### 1. Data Cleaning
In this initial phase, we prepare our datasets for analysis by handling missing values, outliers, and any inconsistencies. This ensures the integrity and quality of our data, setting a strong foundation for the subsequent steps.

### 2. Exploratory Data Analysis (EDA)
The EDA phase allows us to understand the datasets deeply. We identify patterns, anomalies, and correlations that inform our feature engineering process. This phase results in the creation of specific features that are crucial for personalised recommendations.

### 3. Feature Engineering
Leveraging insights gained from EDA, we engineer new features that enhance our model's ability to provide personalised recommendations. This involves the transformation and creation of new data columns that better represent the customers' preferences and behaviors.

### 4. Customer Segmentation
This step involves segmenting H&M's vast customer base into distinct groups based on customer characteristics and transactional behaviors. We employ various clustering techniques such as KPrototypes and KMeans to find the optimal segmentation. Each segment is then analysed and visualised to gain a deeper understanding of the distinct customer profiles.

### 5. Model Development
Finally, we develop the recommendation system using machine learning algorithms. This model is trained and tested on our processed and segmented data, ensuring it can generate accurate and personalized product recommendations for each customer segment. This utilises time-decay-based content filtering, and time-infused collaborative-filtering as individual models. The weights for the 2 models that dictates recommendations for different permutations of customers (based on their clusters) are then predicted by a hybrid lightGBM model, so as to deliver a more personalised recommendation.

## Visualization and Insights
Throughout each phase, we heavily utilise visualisation tools to illustrate our findings and support our decisions. These visual aids are crucial for understanding the complex relationships within the data and validating our approach to personalized recommendations.

We hope you find our project insightful and useful. For any questions or contributions, please feel free to reach out to any of the contributors listed above. Thank you also to the BT4222 team for your guidance in this project. 


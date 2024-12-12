## **Data**

This folder contains runtime output files generated during the project, which were used in various stages of preprocessing, analysis, and visualization.

### **Files Included**
1. **`cleaned_air_india_case_study_articles.csv`**
   - Contains cleaned and preprocessed news articles collected using SerpAPI.
   - Fields include publication date, article title, content, and preprocessing metadata.

2. **`classified_air_india_data.csv`**
   - Dataset with articles labeled by sentiment (positive, negative, neutral).
   - Generated using a fine-tuned DistilBERT model for sentiment analysis.

3. **`keyphrase_comparison.csv`**
   - A comparison of significant key phrases extracted from articles, categorized by pre- and post-privatization periods.

4. **`sentiment_air_india_data.csv`**
   - Sentiment-scored dataset, including polarity and confidence scores.

5. **`pre_post_sentiment_comparison.csv`**
   - A year-wise comparison of sentiment trends for pre- and post-privatization periods.

6. **`final_air_india_data.csv`**
   - Consolidated dataset combining preprocessing, sentiment analysis, and topic modeling results.

7. **`air_india_with_topics.csv`**
   - Final dataset enriched with topic modeling results, including dominant themes identified using LDA.

---

### **Purpose**
The data files play a key role in each stage of the analysis:
- **Preprocessing**: Cleaning and preparing raw news articles for NLP tasks.
- **Sentiment Analysis**: Identifying sentiment polarity (positive, neutral, negative) across time periods.
- **Topic Modeling**: Extracting dominant themes such as fleet modernization, leadership changes, and customer satisfaction.
- **Visualization**: Supporting the generation of charts and graphs to illustrate insights.

---

### **How to Use the Data**
1. **Access Runtime Files**:
   Navigate to the `Data/` folder in this repository to explore the CSV files.

2. **Load and Analyze Data**:
   Use any programming environment (e.g., Python with Pandas) to load and analyze these files.
   ```python
   import pandas as pd

   # Load cleaned data
   cleaned_data = pd.read_csv('Data/cleaned_air_india_case_study_articles.csv')
   print(cleaned_data.head())

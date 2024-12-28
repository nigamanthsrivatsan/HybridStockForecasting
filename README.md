# **Hybrid Stock Forecasting with Sentiment Analysis and Time Series Models**

This study presents a hybrid approach to stock price forecasting by integrating sentiment analysis from social media with traditional time-series forecasting models. By combining VADER and Zero-Shot Text Classification for sentiment analysis with ARIMA, XGBoost, and LSTM for stock price prediction, this study explores the relationship between public discourse volume and the utility of sentiment in stock market predictions.

--- 

## **Overview**
This repository accompanies the research paper titled _"Using LLM to Predict Stock Price: A Hybrid Model Combining Social Media Sentiment and Market Data"_ It includes:
- Datasets for historical stock prices and Tweets.
- Scripts for preprocessing data, sentiment analysis, and implementing the forecasting models.
- Evaluation metrics and visualizations for model performance.
- Detailed Jupyter notebooks documenting the methodology.
- The figures used in the Research Paper coupled with the code used to generate them. 

---

## **Getting Started**
### **Prerequisites**
1. Python 3.8 or higher
2. Libraries specified in `requirements.txt`:
   - Pandas
   - NumPy
   - Scikit-learn
   - TensorFlow
   - XGBoost
   - Seaborn
   - Matplotlib
   - Transformers

### **Installation**
1. Clone this repository:
```
git clone https://github.com/nigamanthsrivatsan/HybridStockForecasting.git
```
2. Install the required libraries:
```
pip install -r requirements.txt
```

### **Usage**
1. **Conduct the exploratory data analysis (optional)**
Begin with the `exploratory_data_analysis.ipynb` notebook to analyze the datasets, identify key patterns, and detect potential issues. This will provide you with a more comprehensive understanding of the dataset.


2. **Preprocess the data:**
Run the `data_preprocessing.ipynb` notebook to clean and prepare the datasets. This is essential for further steps.

3. **Complete the model comparison (optional):**
To compare the 2 sentiment analysis models (VADER & Zero Shot Text Classification) and 3 time series models (ARIMA, XGBoost, and LSTM) and obtain the graphs, tables, and confusion matrices used in the research paper, run the `sentient_models_comparison.ipynb` file. 

4. **Execute the models:**
Run the `model_execution.ipynb` notebook to execute the models and print the RMSEs of the time series models and different feature sets, representing the improvement in accuracy upon adding sentiment. 

---

## **Results**
The models were evaluated on three stocks with varying levels of public discourse:
1. **Tesla (TSLA)**: High public discourse.
2. **Apple (AAPL)**: Moderate public discourse.
3. **Ford (F)**: Low public discourse.

**Key findings include:**
- Sentiment analysis improves accuracy significantly for stocks with higher public discourse, but can cause a slight decrease in accuracy for stocks with lower amounts of public discourse.
- XGBoost shows robust performance across all datasets but is less affected by added sentiment and often treats it like noise.

---

## **Citation**
If you use this repository or its associated research in your work, please cite:
```
Nigamanth Srivatsan. 2025. Hybrid Stock Forecasting: Combining Sentiment Analysis and Time Series Models to Improve Predictive Accuracy. GitHub Repository. https://github.com/nigamanthsrivatsan/HybridStockForecasting
```

---

## **Acknowledgements**
This research was supported by my mentor, Hossein Talebi. Special thanks to all contributors for their guidance and feedback. The Veritas AI program is also acknowledged for providing the platform, resources, and mentorship that enabled the success of this research. Additionally, I would like to extend my gratitude to Kaggle for offering an extensive and easily accessible repository of datasets, which played a crucial role in inspiring this research idea and facilitating its execution.

---

## **License**
This project is licensed under the MIT License. See the [LICENSE.md](LICENSE.md) file for details.

---

## **Contact**
For questions or collaborations, feel free to contact:  
**Nigamanth Srivatsan**  
**Email:** nigamanth.srivatsan@gmail.com  
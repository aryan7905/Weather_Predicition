# 🌦️ Weather Prediction Using Naive Bayes Classifier

## 📋 Project Overview
This project implements a weather prediction model using the Naive Bayes algorithm. The model predicts whether outdoor conditions are suitable for play based on weather features such as outlook, temperature, humidity, and wind.

## 📊 Dataset
The dataset consists of 14 records with the following attributes:
- **Outlook**: Weather outlook (☀️ Sunny, ☁️ Overcast, 🌧️ Rainy)
- **Temp**: Temperature (🔥 Hot, 😌 Mild, ❄️ Cool)
- **Humidity**: Humidity level (💧 High, 🌫️ Normal)
- **Windy**: Wind conditions (💨 t/f representing True/False)
- **Play**: Target variable indicating if conditions are suitable for play (✅ yes/❌ no)

## 🔍 Implementation
The implementation follows these steps:
1. **Data Preprocessing**: 
   - Handling categorical variables using Label Encoding
   - Converting the 't'/'f' string values in the Windy column to 1/0
   
2. **Model Training**: 
   - Splitting data into training and testing sets
   - Training a Gaussian Naive Bayes model
   
3. **Evaluation**: 
   - Calculating accuracy, precision, recall, and F1-score
   - Visualizing results using confusion matrices
   
4. **Prediction**: 
   - Making predictions on new weather conditions
   - Analyzing feature importance

## 📈 Visualizations
The project includes several visualizations to help understand the data and model performance:

### 1. Confusion Matrix
![Confusion Matrix](https://via.placeholder.com/400x300?text=Confusion+Matrix)
*The confusion matrix shows true positives, false positives, true negatives, and false negatives of our model predictions.*

### 2. Feature Distributions by Class
![Feature Distributions](https://via.placeholder.com/600x400?text=Feature+Distributions)
*These histograms show how each feature is distributed across the target classes (yes/no).*

### 3. Feature Importance Analysis
![Feature Importance](https://via.placeholder.com/500x350?text=Feature+Importance)
*This chart shows which features have the most impact on the prediction results.*

## 💻 Requirements
- Python 3.x
- pandas 📊
- numpy 🔢
- scikit-learn 🤖
- matplotlib 📈
- seaborn 🎨

## 🚀 Usage
1. Clone the repository
2. Upload the dataset to your environment or use the provided path
3. Run the Jupyter notebook or Python script

```python
# Example prediction
result = predict_weather("Sunny", "Mild", "Normal", "f")
print(f"Weather prediction: {result}")
```

## 📝 Results
The model demonstrates how the Naive Bayes algorithm can be used for classification tasks with categorical and numerical features. Performance metrics are displayed in the notebook, showing the effectiveness of the model for weather prediction.

Example output:
```
Model Accuracy: 0.8750

Classification Report:
              precision    recall  f1-score   support
         no       0.67      1.00      0.80         2
        yes       1.00      0.67      0.80         3
```

## 🔮 Future Improvements
- Incorporate more weather features
- Use a larger dataset for better generalization
- Experiment with different Naive Bayes variants
- Compare with other classification algorithms

## 📜 License
[MIT](https://choosealicense.com/licenses/mit/)

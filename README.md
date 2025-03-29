# AirQualityPrediction-LSTM
### README for GitHub Repository: Air Quality Prediction Using LSTM Networks

---

# **Air Quality Prediction Using LSTM Networks**

## **Overview**
This project implements Long Short-Term Memory (LSTM) networks to predict air quality by forecasting pollutant levels such as ozone (O₃) and carbon monoxide (CO). The model leverages time-series data from the Environmental Protection Agency (EPA) to provide accurate predictions that can aid in public health interventions and environmental policy-making.

The repository contains:
- Jupyter Notebook for preprocessing, model training, and visualization
- Datasets for ozone and CO levels
- Python scripts for LSTM model implementation
- Visualization plots and analysis results

---

## **Features**
1. **Data Preprocessing**:
   - Handling missing values
   - Scaling features using Min-Max normalization
   - Sequence creation for time-series forecasting

2. **Model Implementation**:
   - LSTM architecture with dropout layers to prevent overfitting
   - Training and validation on sampled data
   - Hyperparameter tuning for optimal performance

3. **Visualization**:
   - Time series plots of actual vs predicted values
   - Error distribution histograms
   - Correlation heatmaps

4. **Results**:
   - Model metrics including Mean Squared Error (MSE) and Mean Absolute Error (MAE)
   - Predictions for ozone and CO levels with detailed visualizations

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/mdshafaque56/AirQualityPrediction-LSTM.git
   cd AirQualityPrediction-LSTM
   ```

2. Install required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Download datasets:
   Place the ozone (`8hour_44201_2024.zip`) and CO (`8hour_42101_2024.zip`) datasets in the `data/` directory.

---

## **Usage**
1. Open the Jupyter Notebook (`AirQualityPrediction.ipynb`) in your preferred environment.
2. Run the cells step-by-step to preprocess data, train models, and visualize results.
3. Visualizations include time series plots, scatter plots, and heatmaps.

---

## **Results**
### Model Performance Metrics:
1. **Ozone Model**:
    - Training MSE: 0.0022 | Validation MSE: 0.0032  
    - Training MAE: 0.0371 | Validation MAE: 0.0446  

2. **CO Model**:
    - Training MSE: 0.0011 | Validation MSE: 0.00084  
    - Training MAE: 0.0241 | Validation MAE: 0.0224  

### Sample Predictions:
- Ozone Levels: [24.09, 24.44, 23.97, ...]
- CO Levels: [25.25, 25.97, 24.41, ...]

### Visualizations:
- Scatter plot showing strong alignment between actual and predicted values.
- Time series forecast demonstrating stable pollutant levels.
- Error distribution centered around zero, indicating unbiased predictions.

---

## **License**
This project is licensed under the MIT License.

---

## **Contributing**
We welcome contributions to improve the project! Feel free to submit issues or pull requests.

---

## **Contact**
For questions or collaborations, reach out to me at www.linkedin.com/in/md-shafaque-37973b280.

GitHub Repository URL:  mdshafaque56/AirQualityPrediction-LSTM

Citations:
[1] https://pplx-res.cloudinary.com/image/upload/v1743232821/user_uploads/SuZouuvrQzMnXDs/Screenshot-2025-03-29-124958.jpg
[2] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/51288755/1742cf91-222e-4861-9b6c-de4252d8a4c7/Air-Quality-Prediction-Using-LSTM-Networks-A-Deep-Learning-Approach.pdf
[3] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/51288755/1742cf91-222e-4861-9b6c-de4252d8a4c7/Air-Quality-Prediction-Using-LSTM-Networks-A-Deep-Learning-Approach.pdf

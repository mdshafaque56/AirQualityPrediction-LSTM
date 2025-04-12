# README: Air Quality Prediction Using LSTM Networks

## **Project Overview**
Air pollution is a growing concern worldwide, and accurate forecasting of pollutant levels is essential for mitigating its adverse effects on human health and the environment. This project leverages Long Short-Term Memory (LSTM) networks to predict ozone (O₃) and carbon monoxide (CO) concentrations based on historical air quality data. By utilizing deep learning techniques, this project aims to provide actionable insights for environmental agencies and urban planners.

---

## **Features**
1. **Dual LSTM Models**:
   - Separate models for predicting O₃ and CO levels.
   - Time-series forecasting with a 24-hour input window.

2. **Data Preprocessing**:
   - Handling missing values using mean imputation.
   - Normalization using MinMaxScaler to scale pollutant levels between 0 and 1.

3. **Visualization**:
   - Geographical distribution of pollutants.
   - Error distributions to analyze model performance.

4. **Evaluation Metrics**:
   - Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² score.

5. **Scalable Architecture**:
   - Easily extendable to other pollutants or additional features like meteorological data.

---

## **Datasets**
The datasets used in this project are sourced from the **EPA Air Quality System (AQS)**. They contain hourly readings of ozone and carbon monoxide concentrations from various monitoring stations across the United States.

### **Dataset Details**:
| Column Name                | Description                              |
|----------------------------|------------------------------------------|
| `Latitude`, `Longitude`    | Geographical coordinates of stations     |
| `Date Local`, `Time Local` | Date and time of observation             |
| `Pollutant_Level`          | Concentration of O₃/CO in ppm           |

---

## **Model Architecture**
The LSTM network architecture consists of:
- **Layers**: Two stacked LSTM layers with 64 neurons in the first layer and 32 neurons in the second layer.
- **Dropout**: Dropout layers with a rate of 0.2 to prevent overfitting.
- **Activation Function**: ReLU for dense layers.
- **Input/Output**: Input sequences consist of 24 time steps; output sequences consist of 1 time step.

### Training Configuration:
| Parameter       | Value               |
|-----------------|---------------------|
| Batch Size      | 64                  |
| Learning Rate   | 0.001 (Adam default)|
| Epochs          | 50                  |
| Validation Split| 20%                 |

---

## **Results**
The models achieved high accuracy in predicting pollutant levels:

### Performance Metrics:
| Metric          | Ozone Model | CO Model |
|------------------|-------------|----------|
| MAE             | 0.037 ppm   | 0.023 ppm|
| MSE             | 0.0022      | 0.0011   |
| R²              | 0.89        | 0.92     |

### Key Visualizations:
1. **Prediction vs Actual Values**:
   - Line plots showing predicted pollutant levels closely matching actual values.
2. **Error Distributions**:
   - Histogram, Q-Q plot, scatter plot, and boxplot highlighting error patterns.

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/air-quality-prediction-lstm.git
   ```
2. Install required Python libraries:
   ```bash
   pip install tensorflow pandas matplotlib seaborn scikit-learn keras-tuner
   ```

---

## **Usage**
1. Download the datasets (`O3_Dataset.csv` and `CO_Dataset.csv`) from the repository(ZIP).
2. Run the Jupyter Notebook (`Model_Project_AI.ipynb`) to preprocess data, train models, and evaluate results.
3. Visualizations will be saved as `.png` files in the `plots` folder.

---

## **Future Work**
1. Integrate meteorological data like temperature, humidity, and wind speed for improved predictions.
2. Explore hybrid models such as CNN-LSTM or attention-based LSTMs for better spatial-temporal analysis.
3. Deploy models for real-time air quality monitoring using TensorFlow Serving.

---

## **License**
This project is licensed under the MIT License.

---

## **Contact**
For queries or collaborations, feel free to reach out via www.linkedin.com/in/md-shafaque-37973b280

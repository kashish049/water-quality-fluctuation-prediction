# Water Quality Fluctuation Prediction

This project aims to predict **Water Quality Index (WQI)** and **Coliform levels** using machine learning models based on environmental and water quality data. The project applies various algorithms to help monitor and predict water quality fluctuations for better environmental management.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Dataset](#dataset)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Model](#model)
7. [Results](#results)
8. [Contributing](#contributing)
9. [License](#license)
10. [Contact](#contact)

## Project Overview
Water quality monitoring is crucial for assessing pollution and ensuring the safety of water for consumption, recreation, and ecosystem health. This project focuses on using historical water quality data to predict future water quality index and coliform (bacteria) levels. The goal is to provide early warnings of water quality degradation.

## Features
- Prediction of Water Quality Index (WQI)
- Prediction of Coliform (Escherichia coli) levels
- Use of real-time and historical environmental datasets
- Visualization of predicted results and actual measurements

## Dataset
We used publicly available water quality datasets that include parameters such as:
- pH level
- Dissolved Oxygen (DO)
- Biochemical Oxygen Demand (BOD)
- Temperature
- Coliform levels
- Water Quality Index (WQI)

You can find the dataset from [National Water Quality Monitoring sources](https://www.epa.gov/national-aquatic-resource-surveys/national-rivers-and-streams-assessment).

## Installation

1. **Clone the repository**:
    ```bash
 https://github.com/kashish049/water-quality-fluctuation-prediction  
    ```

2. **Create a virtual environment** (optional but recommended):
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use: env\Scripts\activate
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Download the dataset** and place it in the `data` directory.

## Usage

1. **Train the model**:
    ```bash
    python train_model.py --dataset data/water_quality_data.csv
    ```

2. **Predict water quality**:
    After training, use the saved model to predict water quality:
    ```bash
    python predict.py --input new_data.csv
    ```

3. **Visualize Results**:
    ```bash
    python visualize_results.py
    ```

## Model

The project applies machine learning algorithms, including:
- K-Nearest Neighbors (K-NN)
- Random Forest
- Gradient Boosting

The model evaluation includes metrics like:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Accuracy for classification tasks (for coliform prediction)

## Results

The following results were achieved on the test set:
- **WQI Prediction**: RMSE of 5.2
- **Coliform Prediction**: Accuracy of 87%

Visualization of the predicted vs actual water quality over time is available through the `visualize_results.py` script.

## Contributing

We welcome contributions! Here's how you can help:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes and commit them (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the NIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions, please contact:
- **Ashish Kumar**: [ashishkumarnith4@gmail.com](mailto:ashishkumarnith4@gmail.com)

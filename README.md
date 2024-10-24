# Binary Classification WebApp using Streamlit

## Overview
This repository contains a **Streamlit WebApp** designed to perform **binary classification** tasks. The primary example used in this project classifies whether a mushroom is **edible** or **poisonous** 🍄, using popular classification algorithms such as **Support Vector Machine (SVM)**, **Logistic Regression**, and **Random Forest Classifier**.

The WebApp allows users to interactively tweak hyperparameters and view important metrics like **Confusion Matrix**, **ROC Curve**, and **Precision-Recall Curve** in real time.

## Features
- **Interactive Interface**: Adjust model hyperparameters and view the impact on performance in real time.
- **Three Models to Choose From**:
  - **Support Vector Machine (SVM)**
  - **Logistic Regression**
  - **Random Forest Classifier**
- **Visualization of Model Performance**:
  - Confusion Matrix
  - ROC Curve
  - Precision-Recall Curve
- **Streamlit Sidebar**: Easy navigation and control over model choices and hyperparameters.
- **Raw Data View**: Toggle the display of the raw data used in classification.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/mushroom-classification-webapp.git
    cd mushroom-classification-webapp
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

## How to Use
1. **Upload the Dataset**: The app uses a preloaded `mushrooms.csv` dataset. However, you can adapt it to any binary classification dataset.
2. **Select a Model**: Choose between SVM, Logistic Regression, and Random Forest.
3. **Set Hyperparameters**: Use the sidebar to adjust hyperparameters like regularization, kernel type, number of trees, etc.
4. **Visualize the Metrics**: The app will display the selected metrics like Confusion Matrix, ROC Curve, and Precision-Recall Curve based on the model's performance.

## Troubleshooting
- If you encounter errors related to **NumPy’s writeable flag**, ensure that the NumPy and scikit-learn libraries are up to date:
    ```bash
    pip install --upgrade numpy scikit-learn
    ```

- If issues persist, try copying the training data before fitting the model:
    ```python
    x_train_copy = x_train.copy()
    y_train_copy = y_train.copy()
    model.fit(x_train_copy, y_train_copy)
    ```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For questions, feel free to reach out to me on [LinkedIn](https://www.linkedin.com/in/your-profile) or submit an issue on GitHub.

Happy Coding! 😄

# dataset
* **Purpose**: Stores raw and processed data used in the project.
  * **data.csv**: Original Spotify dataset containing features like acousticness, danceability, energy, etc.
  * **cleaned_data.csv**: Dataset after cleaning (created in `1_data_processing.ipynb`).
  * **features.csv**: Dataset after feature engineering (created in `2_feature_data.ipynb`).

# models
* **Purpose**: Stores trained models and related artifacts.
  * Trained recommendation models (e.g., clustering models like K-Means).
  * Preprocessing objects such as scalers and encoders for deployment.

# notebook
* **Purpose**: Contains Jupyter notebooks for data preprocessing, model building, and deployment.
  
  * **1_data_processing.ipynb**
    * **Purpose**: Handles data cleaning and initial preprocessing.
      * Load and clean the dataset.
      * Save the cleaned dataset for use in feature engineering.

  * **2_feature_data.ipynb**
    * **Purpose**: Performs feature engineering and transformation.
      * Apply scaling to numerical features.
      * Encode categorical variables.
      * Save the processed feature dataset for modeling.

  * **3_model_building.ipynb**
    * **Purpose**: Builds and evaluates the recommendation model.
      * Implement K-Means for clustering.
      * Train the recommendation model using the feature data.
      * Save the trained model.

  * **4_deployment.ipynb**
    * **Purpose**: Prepares the model for deployment and integrates user preferences.
      * Import trained models and preprocess user preferences.
      * Test and save final deployment-ready artifacts.

  * **widget.ipynb**
    * **Purpose**: Creates an interactive user interface for inputting preferences and receiving recommendations.
      * Include dropdowns for song selection and sliders for feature adjustments.
      * Save user preferences and generate recommendations.

# src
* **Purpose**: Contains Python scripts for data handling, feature processing, and model operations.

  * **data.py**
    * Handles data loading and saving functions.

  * **features.py**
    * Contains functions for scaling, encoding, and feature creation.

  * **models.py**
    * Implements model training, saving, and loading functions.
    * Contains the recommendation function to generate song recommendations based on user preferences.

# users_pref
* **Purpose**: Stores user preference files (optional) for persistence across sessions.
  
# Flight Data Preprocessing for Machine Learning

This repository contains code for preprocessing flight data, preparing it for machine learning tasks. The dataset used in this repository is sourced from a YouTube video by Krish Naik titled ["Feature Engineering and Data Cleaning - End to End Machine Learning Tutorial using Python"](https://youtu.be/fHFOANOHwh8?si=zJbBzeXgqtUV3Vwv).

## Description

The provided Python script performs several preprocessing steps on flight data:

1. **Data Import**: Utilizes pandas to read train and test datasets.
2. **Data Cleaning**: 
    - Extracts date, month, and year from the 'Date_of_Journey' column.
    - Extracts arrival hour and minutes from the 'Arrival_Time' column.
    - Extracts departure hour and minutes from the 'Dep_Time' column.
    - Handles missing values and drops rows with null values.
    - Maps 'Total_Stops' to numerical values.
    - Extracts duration hour and minutes from the 'Duration' column.
    - Converts duration to minutes and replaces null values with 0.
3. **Label Encoding**: Utilizes scikit-learn's LabelEncoder to encode categorical variables such as 'Airline', 'Source', 'Destination', and 'Additional_Info'.

## Usage

1. **Clone the Repository**: Clone this repository to your local machine using the following command:
    ```
    git clone https://github.com/mishra-krishna/Flight-Price-Prediction-EDA
    ```
2. **Install Dependencies**: Ensure you have Python and necessary libraries installed. You can install the required libraries using pip:
    ```
    pip install pandas numpy scikit-learn
    ```
3. **Data Preparation**: Place the 'Data_Train.xlsx' and 'Test_set.xlsx' files in the same directory as the script.
4. **Run the Script**: Execute the script to preprocess the flight data:
    ```
    python flight_preprocessing.py
    ```
5. **Utilize Cleaned Dataset**: After running the script, you can use the cleaned dataset for machine learning tasks.

Feel free to customize the script according to your specific requirements or integrate it into your machine learning pipelines. The cleaned dataset is provided for free and can be integrated with ML models or used for exploratory data analysis.

If you have any questions or suggestions, feel free to reach out or create a pull request.

**Note**: The dataset used in this repository is sourced from Krish Naik's YouTube video for educational purposes.

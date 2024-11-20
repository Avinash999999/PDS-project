import pandas as pd
from sklearn.model_selection import train_test_split

def preprocess_data(input_path, output_path):
    # Load the raw dataset
    data = pd.read_csv(input_path)

    # Example preprocessing steps
    data.dropna(inplace=True)  # Drop rows with missing values
    data = pd.get_dummies(data, drop_first=True)  # Encode categorical features

    # Save the processed data
    data.to_csv(output_path, index=False)
    print(f"Data processed and saved to {output_path}")

if __name__ == "__main__":
    preprocess_data("data/raw_data.csv", "data/processed_data.csv")






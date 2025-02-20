# Fraud Detection System

This project develops a machine learning-based classification system to detect fraudulent insurance claims. The system is designed to process customer and incident data, validate it, preprocess it, train a model on it, and deploy the model to cloud platforms for real-time fraud prediction.

## Project Structure
- **Data Ingestion and Validation**: Validates incoming data files and organizes them based on integrity.
- **Database Management**: Stores validated data in a database for training and prediction.
- **Model Training**: Preprocesses data, clusters it using KMeans, and trains models with the highest AUC score for each cluster.
- **Prediction**: Predicts fraud likelihood on new data batches based on trained models.

## Data Description
The dataset includes features such as:
- `months_as_customer`, `age`, `policy_number`, `policy_bind_date`
- `policy_deductable`, `policy_annual_premium`, `incident_type`
- `total_claim_amount`, `injury_claim`, `property_claim`
- **Target Label**: `fraud_reported` (Y or N)

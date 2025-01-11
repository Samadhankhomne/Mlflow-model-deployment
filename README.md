# Mlflow-model-deployment

# Machine Learning Pipeline with Imbalanced Dataset Handling and MLflow Tracking

## **Dataset**
- Simulated imbalanced binary classification dataset using `make_classification` from `sklearn`.
- Class imbalance handled with **SMOTETomek** (a combination of oversampling and undersampling).

## **Models**
Implemented and compared multiple machine learning models:
1. Logistic Regression.
2. Random Forest.
3. XGBoost with and without SMOTETomek.

## **Experiment Tracking**
Used **MLflow** to:
- Track experiment parameters and metrics (accuracy, recall, F1-score).
- Log and register models.
- Monitor performance metrics for each model run.

## **Model Deployment**
- Registered the best-performing model (`XGBClassifier with SMOTETomek`) in the MLflow Model Registry.
- Transitioned the model to production-ready stages.
- Demonstrated production model loading and prediction.

## **Production Transition**
- Explained how to transition models to production environments.
- Used **MLflowClient** for production model management.

## **Core Libraries and Tools**
1. **scikit-learn** (`sklearn`): Dataset creation, preprocessing, and modeling.
2. **imbalanced-learn**: Handling imbalanced datasets using SMOTETomek.
3. **MLflow**: Model tracking, logging, and deployment.
4. **XGBoost**: Gradient-boosted machine learning models.

---

### **Usage**
1. Clone this repository.
2. Set up MLflow server locally or on a remote machine.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the script to generate datasets, train models, track experiments, and deploy the best-performing model.

### **Repository Highlights**
- **Balanced Dataset Handling**: Uses SMOTETomek to address class imbalance.
- **Model Comparisons**: Evaluates Logistic Regression, Random Forest, and XGBoost.
- **Experiment Management**: Tracks hyperparameters and metrics with MLflow.
- **Model Deployment**: Demonstrates transitioning models to production environments.

### **Future Scope**
- Extend the pipeline to include additional algorithms and techniques.
- Automate the transition to production.
- Integrate with cloud-based MLflow tracking servers for scalability.

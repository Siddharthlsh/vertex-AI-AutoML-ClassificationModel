# vertex-AI-AutoML-ClassificationModel
This uses the Vertex AI classification model evaluation component to evaluate an AutoML Tabular classification model. Model evaluation helps determine your model's performance based on the evaluation metrics and improve the model whenever necessary.

# Overview
This repository works on training a Vertex AI AutoML Tabular classification model and evaluate it through a Vertex AI pipeline job using `google_cloud_pipeline_components`:
### The steps performed include:
- Create a Vertex AI `Dataset`.
- Train an Automl Tabular classification model on the `Dataset` resource.
- Import the trained `AutoML model resource` into the pipeline.
- Run a `Batch Prediction` job.
- Evaluate the AutoML model using the `Classification Evaluation component`.
- Import the classification metrics to the AutoML model resource.
Files to refer to: 
	1. Dataset folder : to download the dataset
        2. Python Notebook: This will act as a tutorial for working with classification model in vertex AI
   

# Introduction to vertexAI
Vertex AI is a machine learning (ML) platform that facilitates the training, deployment, and customization of ML models and AI applications, including large language models (LLMs). It integrates workflows across data engineering, data science, and ML engineering, allowing teams to collaborate using a unified set of tools while leveraging the scalability of Google Cloud to enhance their AI-driven applications.

### Vertex AI provides several options for model training and deployment:
AutoML lets you train tabular, image, text, or video data without writing code or preparing data splits.

Model Evaluation in Vertex AI

Vertex AI provides model evaluation metrics for both predictive AI and generative AI models. The predictive AI evaluation service lets you evaluate model performance across specific use cases.
So,e key metrics provided by the predictive AI model evaluation services include the following
	1. Precision
	2. Recall
	3. AuPRC
	4. Confusion Matrix


# Features
To assess a model with Vertex AI, you need a trained model, batch prediction outputs, and a dataset with ground truth labels. Here’s a standard workflow for model evaluation in Vertex AI:

1. Train a model using either AutoML or custom training options available in Vertex AI.

2. Execute a batch prediction job to produce outputs based on the model.

3. Conduct an evaluation job to measure how well the batch predictions align with the ground truth data.

4. Examine the metrics generated from the evaluation to gauge the model's performance.

5. Refine your model based on insights gained from the evaluation to enhance its accuracy. Multiple evaluations can be conducted to compare different models or versions over time.

# Model evaluation in Vertex AI can be conducted in several ways:

- Initiate evaluations via the Vertex AI Model Registry within the Google Cloud console.
  
- Integrate model evaluations into Vertex AI Pipelines. Utilize these evaluations as part of an automated MLOps workflow, creating pipeline runs and templates that incorporate model assessments.

- Execute the model evaluation component independently or in conjunction with other pipeline components like batch prediction.

# How to Install this example
	1. Clone this project
	2. Set up Google Cloud Consolve
	3. Set up Vertex AI, enable all the plugins
	4. Make sure in Google cloud , your service account have all the permissions
The necessary permissions are: 

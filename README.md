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

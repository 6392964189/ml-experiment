# ml-experiment
import dagshub
dagshub.init(repo_owner='6392964189', repo_name='ml-experiment', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)

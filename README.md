# Simple CI/CD

## Requirements for CI/CD and tooling

  - **ML**: Dataset, train a Model, evaluation
  - **App**: api
  - **Monitoring**: mlflow

  - **Deployment** -> change in data / change in code (model trianing) -> CD
  - **Integration** -> change in code -> run unit tests -> CI

  - **VCS** -> git, dvc (data version control)

  - **CI** -> trigger : on pull request to the "main" branch
  - **CD** -> trigger : on push to the "main" branch

  - **Server for deployment** : local / cloud (AWS)

  - **Containerization** : docker

  - **Orchestration** : kubernetes / docker swarm

  - **Cloud (AWS)** : EC2, S3, ECR, ECS

## Deployment Process

### Basic
  - Install python3 and pip (correct version)
  - Create a python virtual environment (python -m venv .)
  - Get the code (git clone ...)
  - Install dependencies (pip install -r requirements.txt)
  - Start the api (uvicorn src.api:app --host localhost --port 8080)
  
### Docker
  - Pull the latest docker image
  - Stop the current docker container
  - Run docker container from the latest image
  
### Api uri
  - [http://3.110.217.46:8080/](http://3.110.217.46:8080/)
  - [http://3.110.217.46:8080/items/1](http://3.110.217.46:8080/items/1)

## Further reading: 
  - [dvc](https://dvc.org/), [mlflow](https://mlflow.org/), [kubernetes](https://kubernetes.io/), [pytest](https://docs.pytest.org/en/7.4.x/)
  - [https://github.com/lokeshmohanty/mlops-pipeline](https://github.com/lokeshmohanty/mlops-pipeline)

# Sample Kubeflow Pipelines

This repo includes some sample pipelines that have been taken from [Kubeflow Pipelines repo](https://github.com/kubeflow/pipelines) and modified in some cases to work on minikf & AWS.

All pipelines come with two files:

- `.py`: source code of peipeline
- `.yaml`: pipeline artefact to be uploaded to kubeflow pipeline

## Creating Pipeline

If you would like create a new pipeline or make changes to existing ones, do the following:

1. Ensure that Python 3 is installed on your machine
1. Create virtual environment: `python3 -m venv pipeline`
1. Activate environment: `source pipeline/bin/activate`
1. Install [kfp SDK](https://www.kubeflow.org/docs/pipelines/sdk/install-sdk/): `pip3 install kfp --upgrade --user`
1. Navigate to folder with the `.py` pipeline source
1. Compile the pipeline by running `python3 pipeline.py`
1. This will create a `pipeline.py.yaml` that can be uploaded to kubeflow 

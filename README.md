# Snakemake GCP Kubernetes + GCS

Run `pixi run snake` to test the Snakemake pipeline locally

For GCP:
Run `gcloud config set project orcestra-833613` to set the GCP project
Run `pixi run snake-gcp` task to use GCP Storage and Kubernetes

- Assumes you have a kubernetes cluster running and `kubectl` configured locally
or else youll get the `kubernetes.config.config_exception.ConfigException: Service host/port is not set.`
error
- Assumes `orcestradata` bucket exists in GCP Storage

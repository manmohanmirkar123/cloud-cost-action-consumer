# Test Consumer Repo

This repository is a sample consumer for the `cloud-cost-estimator-action`.

## What It Does

- Contains a small multi-cloud Terraform example in `terraform/`
- Includes sample AWS, Azure, and GCP resources for cost estimation
- Runs the custom action from `manmohanmirkar123/cloud-cost-estimator-action`
- Prints the action outputs in the workflow logs
- Uploads the cost report artifact to the GitHub Actions UI through the action itself

## Required Secret

Add this repository secret before running the workflow:

- `INFRACOST_API_KEY`

## Workflow

The workflow file is:

- `.github/workflows/test-cost-action.yml`

## Example Resources

The sample Terraform configuration currently includes:

- `aws_instance.example`
- `azurerm_resource_group.example`
- `google_storage_bucket.example`

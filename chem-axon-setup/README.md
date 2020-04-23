<h1 id='HPG9CA7YL2o'>ChemAxon Compound Registration DB to AWS Data Lake</h1>

The folder/repo holds the codebase for creating AWS Infrastructure and ETL job for loading data from existing Compound
Registration Database to S3 in a scheduled way.<br/>

### Pre-requisites

- AWS RDS Instance which holds Compound Registration Data.

- AWS Details like VPC, Subnet, AZ's, RDS Connection Details to be filled in configs/deploy_config.env file for each env.

- Python and CDK installed.

### Steps to be executed

- Download the codebase locally.
- Ensure the AWS profiles are set for use.
- Fill the details in configs/deploy_config.env
- Start the deployment by running :
  ```bash
  cd chem-axon-setup
  sh deploy.sh <env> # env is the same variable used in deploy_config.env in lower case.
  ```

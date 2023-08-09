# azure-static-web-app
Creating a code deployment for azure static web apps with validation in DevOps using different staging and production environments.

## Prerequisites:
- Azure static web app.
- Deployment token for the static web app.
- Authorisation to deploy code to your static web app.
- Azure DevOps project.


## Running the pipeline:
- In your Azure DevOps project under Library create a variable group and add the deployment token. 
- Create your pipeline using the pipelines/azure-pipeline.yml file.
- Add variables to the pipeline for the recently created secret name-of-token, your-variable-group and the user-email.
- Run the pipeline.
- Once the deployment stage had finished you should be able to see a staging environment in your static web app.
- To go to the production stage approve the validation step.
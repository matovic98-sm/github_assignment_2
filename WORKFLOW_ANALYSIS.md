# GitHub Actions Workflow Analysis

## What triggers this workflow to run?
The workflow is run when code is pushed to the main branch or when a pull request is created targeting the main branch. 
## What are the four main steps this workflow performs?
The four main steps the workflow performs are:
- Checkout Code: This retrieves the repository files so they can be accessed by the workflow.
- Validate HTML: This checks the HTML files for errors and ensures the code follows the proper HTML standards.
- Check Links: This checks the website for broken links or invalid links.
- Upload Artifact: This packages and uploads the websites files so they are available for deployment.
## What does the "Checkout code" step do and why is it necessary?
The "Checkout code" step downloads the repository files and is necessary because the workflow needs access to the projects files to be able to perform tasks such as validating HTML, checking links, and preparing the website for deployment.
## What is the purpose of the environment configuration?
The environment configuration identifies where the website will be deployed by setting the environment name to github-pages and provides the URL to the published website. 
## How does this automated deployment improve reliability compared to manual deployment?
Automated deployment leads to improved reliability compared to manual deployment because it allows for systemic checks each time changes are pushed to the main branch. This reduces the chance that errors make it into the deployment phase and it makes the process more consistent because someone doesn't have to manually validate the HTML, check links, and prepare the website for deployment.
## What would happen if you pushed code to a different branch (not main)?
If I had pushed code to a different branch other than the main branch, the workflow would not automatically run. This is because it is configured to only be triggered when someone tries to push changes to the main branch. 
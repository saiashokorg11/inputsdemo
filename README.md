# inputs and perameters:

## Manual Multi-Environment Deployment
This project uses a single GitHub Actions workflow to manage deployments across different environments. To ensure control over the release process, deployments are triggered only manually via the GitHub interface.
 
  "Hear we have using the different environmetns in single workflow."
  
  Note : In this situation adding the env's in workflow only using manual depolyment only (workflow_dispatch) not using push_requests 

## Configuration Requirements
Before running the workflow, ensure you have:
"GitHub Environments": Configured in Settings > Environments (e.g., Development, Staging, Production).
"Workflow dispatch": The workflow must exist in your repository's default branch to be visible in the Actions tab. 

  "Actions --> workflow(inputsdemo) --> Run_works --> select the values (env's, tags and chouise)"
  
## How to Trigger the Deployment
Follow these steps to manually deploy to a specific environment with your chosen parameters:
"Navigate to Actions": Go to the Actions tab at the top of your GitHub repository.

"Select Workflow": On the left sidebar, click the workflow named inputsdemo.

"Open Run Menu": Click the Run workflow dropdown button on the right side of the page.

# Configure Inputs:
  "Environment": Select your target environment from the dropdown.
  
  "Tags": Enter the specific Git tag or version you wish to deploy.
  
  "Choice Options": Choose from the predefined configuration options provided in the menu.
  
  "Start Deployment": Click the green Run workflow button to initiate the manual job.

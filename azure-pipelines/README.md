# Azure Pipelines Configuration

This folder contains the configuration files for setting up and running continuous integration (CI) and continuous delivery (CD) pipelines using Azure Pipelines for the project.

## Overview

Azure Pipelines is a cloud-based service provided by Microsoft Azure that allows you to automate your build, test, and deployment processes. This repository includes the necessary configuration files to define and execute pipelines tailored for this project.

## Files

### 1. azure-pipelines/qa.yml

This YAML file defines the deployment configuration for the development environment. It specifies the deployment steps, environment variables, and any other necessary configurations for deploying to the development environment.

### 2. azure-pipelines/production.yml

Similar to the dev.yml file, this YAML file defines the deployment configuration for the production environment.

## Getting Started

### 1. Azure Pipelines Setup:

- Set up an Azure DevOps project and repository.
- Create a new pipeline in Azure Pipelines and link it to this repository.

### 2. Pipeline Configuration:

- Adjust the azure-pipelines.yml file to suit the specific requirements of your project.
- Modify the deployment configuration files (dev.yml, prod.yml) in the deployment/environments/ folder.

### 3. Environment Variables:

- Define any sensitive information or configuration parameters as secret variables in Azure Pipelines.

### 4. Trigger Pipeline:

- Push changes to your repository or manually trigger the pipeline in Azure Pipelines to initiate the CI/CD process.

## Environment configuration
-  VS CODE settings.json 
```json
{
  "[yaml]": {
    "diffEditor.ignoreTrimWhitespace": false,
    "editor.autoIndent": "advanced",
    "editor.defaultFormatter": "redhat.vscode-yaml",
    "editor.insertSpaces": true,
    "editor.quickSuggestions": {
      "comments": false,
      "other": true,
      "strings": true
    },
    "editor.tabSize": 2
  },
  "files.associations": {
    "**/azure-pipelines/**/*.yaml": "azure-pipelines",
    "**/azure-pipelines/**/*.yml": "azure-pipelines",
    "**/charts/*.yaml": "helm",
    "*.liquid": "liquid",
    "*.yaml": "yaml"
  }
}
```

## References

- https://youtu.be/e0bF1LlclEs?si=1Kp6bdtF_QU2vLTs

## Contributing

Contributions to improve the CI/CD process are welcome. Please fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License.

## Contact

For any questions or concerns, please contact the project maintainers or open an issue in the repository.

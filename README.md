### Everything as Code with Azure DevOps

Azure DevOps is Micrososft's native solution which enables end-to-end software delivery. Yes, this includes the CI/CD capability with number of great features to go hand-in-hand for a comprehensive process.

The attached repository holds sample pipelines which caters the following scenarios. 

```
Build 
| * Infrastructure
| * Application


Build 
| * Infrastructure
| * Application
|
|-> develop
|      |
|      |-> Deploy DEV (Primary Region)
|      |     * Primary Region
|      |
|      |-> Deploy QA (Primary Region)
|      |     * Primary Region


Build 
| * Infrastructure
| * Application
|
|-> develop
|      |
|      |-> Deploy DEV (Primary Region)
|      |     * Primary Region
|      |
|      |-> Deploy QA (Primary Region)
|      |     * Primary Region
|
|- master
|      |
|      |-> Deploy UAT
|      |     * Primary Region
|      |
|      |-> Deploy STG
|      |     * Primary Region
|      |
|      |-> Deploy PROD
|      |     * Primary Region
|      |     * Secondary Region

```

### build.yml - Build Status


| Branch        | Status        |
| ------------- |:-------------:|
| `master`      | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=master)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=11&branchName=master)|
| `develop`     | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=develop)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=11&branchName=develop)|

### build-dev.yml - Build and Deploy to single environment Status

| Branch        | Status        |
| ------------- |:-------------:|
| `master`      | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=master)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=14&branchName=master)|
| `develop`     | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=develop)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=14&branchName=develop)|

### azure-pipelines.yml - Deployment Status of the full pipeline

| Branch        | Status        |
| ------------- |:-------------:|
| `master`      | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=master)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=9&branchName=master)|
| `develop`     | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=develop)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=9&branchName=develop)|

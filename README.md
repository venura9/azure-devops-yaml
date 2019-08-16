### Everything as Code with Azure DevOps

Azure DevOps is Micrososft's native solution which enables end-to-end software delivery. Yes, this includes the CI/CD capability with number of great features to go hand-in-hand for a comprehensive process.

YAML Pipelines brought in the Configuration as Code aspect to pipelines as all the pipelines (CI/CD) can be version controlled. 

Multi-Stage piplines (Currently a Preview Feature - Aug/2019) is the latest addition to the set of features, which is the core concept for this repository.

The attached repository holds sample pipelines which caters the following scenarios. 

#### Meetup slides supporting the repository can be found here..

[![slides-on-slideshare](https://image.slidesharecdn.com/everythingascodewithazuredevops-190816021609/95/everything-as-code-with-azure-devops-1-638.jpg)](//www.slideshare.net/venura1/everything-as-code-with-azure-devops)

#### Scenarios Covered

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

### Build Status

#### [Build Only](build.yml) 


| Branch        | Status        |
| ------------- |:-------------:|
| `master`      | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=master)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=11&branchName=master)|
| `develop`     | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=develop)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=11&branchName=develop)|

#### [Build > DEV](build-dev.yml) 

| Branch        | Status        |
| ------------- |:-------------:|
| `master`      | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=master)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=14&branchName=master)|
| `develop`     | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=develop)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=14&branchName=develop)|

#### [Build> Deply to Multiple Environments](azure-pipelines.yml) 

| Branch        | Status        |
| ------------- |:-------------:|
| `master`      | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=master)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=9&branchName=master)|
| `develop`     | [![Build Status](https://dev.azure.com/theToDoCompany/theToDoApplication/_apis/build/status/venura9.azure-devops-yaml?branchName=develop)](https://dev.azure.com/theToDoCompany/theToDoApplication/_build/latest?definitionId=9&branchName=develop)|

CI/CD Pipeline Documentation

This documentation describes the CI/CD pipeline that has been set up to automate the build, test, and deployment processes of the Balanceè platform to a staging environment.To ensure that the platform's code is continuously integrated and delivered efficiently, the pipeline makes use of GitHub Actions as its CI/CD tool..

CI (Continous Integration) and CD (Continous Deployment) ensures that the code latest are automatically tested and deployed to the staging environment.

Firstly, i created a github repository (devops-internship-task),then i activated github actions by creating a ci-cd YAML file (.github/workflows/ci-cd.yml). Secondly, i added a server.js file to serve as the primary entry point for Node.js based application. the server.js imports the dependency (express), sets up the instance and defines the route to handle incoming requests.
Thirdly, i created a dockerfile,

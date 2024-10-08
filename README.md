CI/CD Pipeline Documentation

This documentation describes the CI/CD pipeline that has been set up to automate the build, test, and deployment processes of the Balanceè platform to a staging environment.To ensure that the platform's code is continuously integrated and delivered efficiently, the pipeline makes use of GitHub Actions as its CI/CD tool..

- CI (Continous Integration) and CD (Continous Deployment) ensures that the code latest are automatically tested and deployed to the staging environment.

- I created a github repository (devops-internship-task),then i activated github actions by creating a ci-cd YAML file (.github/workflows/ci-cd.yml). 

- I added a server.js file to serve as the primary entry point for Node.js based application. the server.js imports the dependency (express), sets up the instance and defines the route to handle incoming requests.

- I created a dockerfile, that package and runs the server.js file in a docker container. The containerized server.js environment is then used for building, testing and deployment.
Pipeline Steps:

1. Build
- Checkout code from GitHub repository.
- Build Docker image using Dockerfile.

2. Test
- Run automated tests on the built image.

3. Deploy
- Push built image the container registry ( Docker Hub).
- Deploys the image to the production environment.

Pipeline Configuration

.github/workflow: The workflow file specifies the trigger, environment variables, and pipeline steps.

Environment variable
secrets.DOCKER_USERNAME : My docker username
secrets.DOCKER_PAT : Docker PAT

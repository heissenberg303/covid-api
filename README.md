# Covid-19 stats summarize

> count total number of covid cases by each provinces and age range group such as '0-30, 31-60, 61+, or NA'.

### Components
- Port and Adapter Design Pattern
- Go with Gin framework
- Unit testing using Testify
- Create Dockerfile
- Gitlab CI pipeline including security scan(SAST, Container Scanning, Secret Detection, Dependency Scanning), Code Quality Check, Build, and Deploy to ArgoCD.

## How to run
### Use Docker
1. ```docker build -t covid .```
2. ```docker run -it --rm covid```
3. ```docker exec -it <mycontainer> bash```

### Sample curl
> ```curl 'localhost:8080/covid/summary'```

### Deployment
1. Provision ArgoCD in Kubernetes cluster [repository](https://github.com/heissenberg303/argo-deployment)
2. Deployment in Kustomization [repository](https://github.com/heissenberg303/covid-app-kustomize)

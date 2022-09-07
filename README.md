# DevOps CI/CD Pipeline

- Set up a CI/CD pipeline to build and deploy a real-time java project on AWS cloud
- CI: Jenkins pulls code from Github, builds code with Maven, and sends artifacts to Ansible. Ansible creates a docker image and pushes it to Dockerhub
- CD: Kubernetes pulls docker image from Dockerhub, generates a pod set with 3 replicas using rolling update strategy, and deploys service with load balancer

# containarization and Container Orchestration Project
# Aim:
Containerization of a simple static website (HTML and CSS) application for a company's landing page using docker and deploying it to a kubernetes cluster, and access it through Ngnix.
## Setting up website
- The project directory was created 
![project-dir](./img/1.new-directory.png)
- The HTML file was created usin `vim` syntax.
![HTML-file](./img/2.index.html-file.png)
- The CSS file was created.
![css-file](./img/3.style-css-file.png)
## Git initialization
- Git repository was initialized in the capstone project directory by creating the directory from repository and cloning it on bash.
![git-init](./img/4.git-init.png)
## Git commit
- The added HTML and CSS file was added, commit and push to remote repository.
![git-commit](./img/5.git-commit.png)
## Dockerization of the application
- Dockerfile specifyig Ngnix as a base image was created.
![dockerfile-create](./img/6.creating-docker-file.png)
- codes for website was added to the HTML file.
![html-content](./img/10.html-content.png)
- codes for website was added to the css file.
![css-content](./img/11.style-css.png)
- The HTML and CSS files were copied into Nginx HTML directory.
![html-css-copy](./img/8.copying-html-css-files-into-nginx-file.png)
- The docker image was built.
![docker-build](./img/7.building-docker-image.png)
## Pushing the docker image to docker hub
- The docker hub was logged in.
- The docker image was tag.
![docker-image-tag](./img/12.taging%20the%20docker%20image.png)
- Docker image was push to docker hub.
![push-docker-img](./img/13.push-to-docker-hub.png)
## Setting up kind kubernetes cluster
- The kind kubernete was in docker.
![install-kubernetes](./img/14.install%20kind.png)
- Creating kind cluster.
![kind_created](./img/15.creating-kind-cluster.png)
## Deploying Kubernetes
- Creating YAML file for kubernetes deployment.
![yaml-file_created](./img/16.create-yaml-file.png)
- The kubernetes deployemnt was deploy to the kind cluster using `kubectl apply --f services.yaml` syntax
![kube-deploy](./img/17.apply-kubernete-deployment.png)
- The kubernetes deployment was verify using    `kubectl get services` syntax. 
![deploy-verification](./img/18.verifying-the-deploy-kubernetes.png)
## Accessing the Application
- The created appication was port-forwarded to the service to access application locally.
![port-forwarding](./img/19.port-forwarding-the-deployment.png)
- Visualizing the frontend application on the browser using the port '8080'

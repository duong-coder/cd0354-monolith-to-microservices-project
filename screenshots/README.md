# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![DockerHub showing containers that you have pushed](/screenshots/dockerhub_image_pushed.png)

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
[![Build Status](https://app.travis-ci.com/duong-coder/cd0354-monolith-to-microservices-project.svg?token=VgcNBSrWsgdX7GqGJRUK&branch=main)](https://app.travis-ci.com/duong-coder/cd0354-monolith-to-microservices-project)

* Travis CI showing a successful build and deploy job
![Travis CI showing a successful build and deploy job](/screenshots/travis_ci_success.png)

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![Kubernetes pods](/screenshots/get_pods.png)

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![Kubernetes services](/screenshots/describe_services_01.png)
![Kubernetes services](/screenshots/describe_services_02.png)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![Kubernetes hpa](/screenshots/get_hpa.png)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![Kubernetes logs](/screenshots/get_logs.png)

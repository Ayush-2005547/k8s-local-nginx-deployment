# Kubernetes Task 5: Local Deployment Using Docker Desktop

## Overview

This project demonstrates the deployment and management of a basic NGINX web application on a local Kubernetes cluster using Docker Desktop. The task was completed as part of a practical Kubernetes learning exercise.

## Objectives

- Set up a local Kubernetes cluster
- Create a deployment using YAML
- Expose the deployment using a NodePort service
- Interact with the cluster using `kubectl` commands
- Scale the application
- Retrieve logs and describe Kubernetes resources

## Tools and Technologies

- Kubernetes (Docker Desktop with Kubernetes enabled)
- kubectl
- Docker
- YAML
- NGINX container image

## Files Included

| File             | Description                                              |
|------------------|----------------------------------------------------------|
| `deployment.yaml`| Defines the NGINX deployment with the desired replicas   |
| `service.yaml`   | Exposes the deployment using a NodePort service          |
| `README.md`      | Documentation of the project                             |
| `screenshots/`   | Contains screenshots of command outputs and results      |

## Kubernetes Commands Used

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl get pods
kubectl get svc
kubectl scale deployment nginx-deployment --replicas=4
kubectl describe pod <pod-name>

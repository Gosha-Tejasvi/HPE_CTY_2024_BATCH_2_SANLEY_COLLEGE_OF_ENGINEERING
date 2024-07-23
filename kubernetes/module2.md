## Module 2: Deploy an App with kubectl

### Objectives

- Learn about application Deployments in Kubernetes.
- Deploy your first app on Kubernetes with `kubectl`.

### Kubernetes Deployments

In Kubernetes, a Deployment manages the lifecycle of your application instances. It provides features for deploying new versions of your application, scaling it, and ensuring high availability by automatically replacing failed instances.

### Deploying Your First Application

To deploy an application on Kubernetes using `kubectl`, follow these steps:

1. **Verify kubectl Configuration**

   Ensure that `kubectl` is configured to talk to your Kubernetes cluster by checking its version:

   ```bash
   kubectl version
```
This command should display both the client and server versions of kubectl.

Deploy the Application

Use the following command to deploy a sample application (kubernetes-bootcamp) using a specific Docker image:

```bash
kubectl create deployment kubernetes-bootcamp --image=gcr.io/google-samples/kubernetes-bootcamp:v1
```

This command instructs Kubernetes to create a Deployment named kubernetes-bootcamp using the Docker image gcr.io/google-samples/kubernetes-bootcamp:v1.

Verify Deployment

After deploying, verify that the Deployment was successful by listing the deployments:

```bash
kubectl get deployments
```
This command lists all deployments in your Kubernetes cluster, including the kubernetes-bootcamp Deployment.

Conclusion
Congratulations! You've successfully deployed your first application on Kubernetes using kubectl. Continue to Module 3: Explore Your App to learn more about interacting with your deployed application and understanding its runtime environment.

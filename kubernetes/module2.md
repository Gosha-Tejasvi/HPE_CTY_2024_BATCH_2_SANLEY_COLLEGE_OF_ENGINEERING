# Module 2: Deploy an App

In this module, we will deploy our first application on Kubernetes using `kubectl`.

## Objectives

- Deploy a containerized application on Kubernetes.
- Understand how Kubernetes schedules applications on available nodes.

## Deploying Your First Application

To deploy an application on Kubernetes, use the following command. Replace `<image>` with the full repository URL if the image is hosted outside Docker Hub.

```bash
kubectl create deployment kubernetes-bootcamp --image=gcr.io/google-samples/kubernetes-bootcamp:v1
```
This command deploys the kubernetes-bootcamp application using the specified Docker image gcr.io/google-samples/kubernetes-bootcamp:v1.

Verify Deployment
After deploying, verify that the deployment was successful by checking the deployments:

copycode
Copy code
kubectl get deployments
This command will list all deployments in your Kubernetes cluster, showing information about the kubernetes-bootcamp deployment.

Conclusion
Congratulations! You've successfully deployed your first application on Kubernetes using kubectl. Continue to Module 3: Explore Your App to learn more about interacting with your deployed application and understanding its runtime environment.

vbnet
Copy code

### Explanation:

- **`copycode` Block**: By using ```copycode ... ```, you indicate to users that this block of code is meant to be copied and executed. This is a common convention in technical documentation to distinguish executable commands.
- **Instructions**: Provide clear instructions before each code block to explain what the command does and any necessary context.
- **Link to Next Module**: Always link to the next module or section to guide users through the tutorial sequentially.

This format will help users understand how to deploy an application on Kubernetes using `kubectl` while maintaining clarity and ease of use in your documentation.

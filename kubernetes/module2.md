# Module 2: Deploy an App

In this module, we will deploy our first application on Kubernetes using `kubectl`.

## Objectives

- Deploy a containerized application on Kubernetes.
- Understand how Kubernetes schedules applications on available nodes.

## Deploying Your First Application

To deploy an application on Kubernetes, we use the `kubectl create deployment` command. This command creates a deployment object which manages a replica set to ensure the specified number of pod replicas are running at any given time.

### Steps

1. **Deploy the Application**

   Use the following command to deploy an application. Replace `<image>` with the full repository URL if the image is hosted outside Docker Hub.

   ```bash
   kubectl create deployment kubernetes-bootcamp --image=gcr.io/google-samples/kubernetes-bootcamp:v1
 ```
This command deploys the kubernetes-bootcamp application using the specified Docker image gcr.io/google-samples/kubernetes-bootcamp:v1.

Verify Deployment

After deploying, verify that the deployment was successful by checking the deployments:

bash
Copy code
kubectl get deployments
You should see output confirming the deployment, including the number of replicas running.

Explore Further

Kubernetes automatically searches for a suitable node to run the application, schedules it, and configures the cluster for resilience (e.g., rescheduling on failure).

Conclusion
Congratulations! You've successfully deployed your first application on Kubernetes using kubectl. In the next module, we will explore how to interact with and manage your deployed application further.

Continue to Module 3: Explore Your App to learn more about interacting with your deployed application and understanding its runtime environment.

vbnet
Copy code

### Notes:

- Ensure to replace `<image>` in the deployment command with the actual Docker image repository URL if deploying an image from a different source than Docker Hub.
- Provide clear and concise instructions for each step to guide users effectively through the deployment process.
- Link to the next module (`module3.md`) to encourage users to proceed with the tutorial in a structured manner.

By following this structure, users will be able to deploy their first application on Kubernetes and verify its deployment status using `kubectl`. This sets a foundation for further exploration and learning in subsequent modules.

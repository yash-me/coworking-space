GitHub Repository: [Github](https://github.com/yash-me/coworking-space/)

To create Docker images for your project, follow these steps:

Modify your code as needed and push the changes to your GitHub repository.
An automated CodeBuild process will trigger when it detects changes in the repository.
This CodeBuild process will build new Docker images and push them to your Amazon Elastic Container Registry (ECR) repository on AWS.
Once the image is created, retrieve the image link.
To set up a Kubernetes cluster and node group, follow the instructions provided in your course lectures.

For your PostgreSQL database, you can use Helm to install and configure it. Make sure to test the database connection and import the seed data into the database. You can refer to the configuration section in your project for guidance.

Next, extract the database password and store it in a secret.yaml file.

Use the following command to create new pods and services for your application:

`kubectl apply -f deployment/  # Navigate to your project folder first`

Check the status of your pods to ensure they are running and ready:

`kubectl get pods`

You can also call the API endpoint to test your application. If needed, check the application logs using the following command:

`kubectl logs <podname>`
These steps will help you build, deploy, and monitor your microservices application.

Amazon Elastic Container Service (Amazon ECS) is a fully managed container orchestration service that helps you easily deploy, manage, and scale containerized applications. As a fully managed service, Amazon ECS comes with AWS configuration and operational best practices built-in. It's integrated with both AWS and third-party tools, such as Amazon Elastic Container Registry and Docker. This integration makes it easier for teams to focus on building the applications, not the environment. You can run and scale your container workloads across AWS Regions in the cloud, and on-premises, without the complexity of managing a control plane.

There are three layers in Amazon ECS:

- Capacity - The infrastructure where your containers run
    
- Controller - Deploy and manage your applications that run on the containers
    
- Provisioning - The tools that you can use to interface with the scheduler to deploy and manage your applications and containers

![[Pasted image 20240216154736.png]]




### Summary of Components:
A container is a standardized unit of software development that holds everything that your software application requires to run. This includes relevant code, runtime, system tools, and system libraries. Containers are created from a read-only template that's called an _image_. Images are typically built from a Dockerfile. A Dockerfile is a plaintext file that specifies all of the components that are included in the container. After they're built, these images are stored in a _registry_ such as Amazon ECR where they can be downloaded from.

After you create and store your image, you create an Amazon ECS task definition. A _task definition_ is a blueprint for your application. It is a text file in JSON format that describes the parameters and one or more containers that form your application. For example, you can use it to specify the image and parameters for the operating system, which containers to use, which ports to open for your application, and what data volumes to use with the containers in the task. The specific parameters available for your task definition depend on the needs of your specific application.

After you define your task definition, you deploy it as either a service or a task on your cluster. A _cluster_ is a logical grouping of tasks or services that runs on the capacity infrastructure that is registered to a cluster.



### How does ECS work?

Task:

have two components.
**ECS Containers instance** 

In AWS ECS (Elastic Container Service), an ECS Container Instance is essentially an Amazon EC2 (Elastic Compute Cloud) instance that has been registered with the ECS cluster and is capable of running Docker containers.and also runs the AWS Container agent.
**Container agent:**
It is responsible for comuncation between ECS and the instances.
Also provides the status of running containers.
Collect Clusters and make sure the version is available.

**ENI:**
ENI stands for Elastic Network Interface. An ENI is a virtual network interface that you can attach to an EC2 instance in your Virtual Private Cloud (VPC). ENIs are fundamental components of networking in AWS, and they enable EC2 instances to communicate with other resources within the VPC and the broader internet.
How the contianer interacts with EC2 Host and with the internet


**Task Defination:**
  
In Amazon ECS (Elastic Container Service), a task definition is a blueprint or configuration file that describes how a Docker container should be launched as part of a task. It defines various parameters such as which Docker image to use, how much CPU and memory to allocate, networking configuration, environment variables, and more.
#### Fargate Launch Type: 
It is a compute engine in ECS that user to launch the containers  without monitor  clusters .
AWS Manages the conatianers for you.
EC2 Launch Type:




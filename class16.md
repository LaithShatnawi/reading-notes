# AWS: Cloud Servers

## AWS EC2

### 1.What is an EC2 Instance?

Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. You can add capacity (scale up) to handle compute-heavy tasks, such as monthly or yearly processes, or spikes in website traffic. When usage decreases, you can reduce capacity (scale down) again.

### 2.Name 2 use cases for EC2.

General Purpose

Compute Optimized

### 3.Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.

One of the biggest advantages is the flexibility to change underlying EC2 instances. As the traffic or demand increases, we can easily change EC2 instances without any issues.

## EC2 For Humans

### 1.Where can we find EC2 on the AWS Console?

in the console click on EC@ under compute tab, then click at launch instance to creat a new instance.

### 2.Explain the general difference between T2 Micro and XL.

T2 instances are a low-cost, general purpose instance type that provides a baseline level of CPU performance with the ability to burst above the baseline when needed.

t2.micro	1	6	1	EBS-Only   Low to Moderate

t2.2xlarge	8	81	32	EBS-Only	Moderate

### 3.Explain a “Compute Cycle” to a non-technical friend.

 a "compute cycle" refers to the basic unit of operation that a computer performs when it carries out tasks or calculations. It's like a single step or action that the computer takes to process information and produce results.

 Imagine you have a recipe to bake a cake. Each step you take, such as mixing the ingredients, pouring the batter into a pan, and putting it in the oven, represents a compute cycle. Similarly, a computer performs a series of steps to complete a task.

## Elastic Beanstalk

### 1.What is Elastic Beanstalk?

its an amazaon web service that let you quickly deploy and manage applications in the AWS Cloud without having to learn about the infrastructure that runs those applications. Elastic Beanstalk reduces management complexity without restricting choice or control. You simply upload your application, and Elastic Beanstalk automatically handles the details of capacity provisioning, load balancing, scaling, and application health monitoring.

### 2.Describe the relationship between EC2 and Elastic Beanstalk.

Elastic Beanstalk and EC2 cater to different use cases and requirements. Elastic Beanstalk is ideal for developers who want to focus on writing code and deploying applications without worrying about infrastructure management. It provides a simplified, managed environment with automatic scaling and integration with other AWS services. However, it may not support all application requirements and can lead to vendor lock-in.

EC2, in contrast, offers greater flexibility and control over the underlying infrastructure, making it suitable for a wider range of applications and custom configurations. It provides various pricing models to optimize costs based on usage patterns. However, it comes with a steeper learning curve and increased management overhead.

### 3.Name some benefits of using Elastic Beanstalk.

Simplified Management: automates the provisioning, monitoring, and maintenance of the underlying infrastructure, allowing developers to focus on writing code and deploying applications.

Automatic Scaling: automatically scales the application based on predefined rules and metrics, ensuring optimal performance during traffic spikes.

Integrated Services: integrates with other AWS services, such as RDS, S3, and CloudWatch, providing a seamless experience for developers.

Customization: although it manages the infrastructure, developers can still customize the environment using configuration files and custom AMIs.
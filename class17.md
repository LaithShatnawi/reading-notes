# AWS: S3 and Lambda

## AWS S3

### 1.What is Amazon S3?

Amazon Simple Storage Service (Amazon S3) is an object storage service offering industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can store and protect any amount of data for virtually any use case, such as data lakes, cloud-native applications, and mobile apps. With cost-effective storage classes and easy-to-use management features, you can optimize costs, organize data, and configure fine-tuned access controls to meet specific business, organizational, and compliance requirements.

### 2.Name some use cases for Amazon S3.

Build a data lake

Back up and restore critical data

Archive data at the lowest cost

Run cloud-native applications

### 3.Name some benefits of using Amazon S3.

With S3 bucket names, prefixes, object tags, and S3 Inventory, you have a range of ways to categorize and report on your data, and subsequently can configure other S3 features to take action. Whether you store thousands of objects or a billion, S3 Batch Operations makes it simple to manage your data in Amazon S3 at any scale.

In addition to these management capabilities, use Amazon S3 features and other AWS services to monitor and control your S3 resources. Apply tags to S3 buckets to allocate costs across multiple business dimensions (such as cost centers, application names, or owners), then use AWS Cost Allocation Reports to view the usage and costs aggregated by the bucket tags.

Amazon S3 offers flexible security features to block unauthorized users from accessing your data. Use VPC endpoints to connect to S3 resources from your Amazon Virtual Private Cloud (Amazon VPC) and from on-premises.

## AWS Lambda Basics

### 1.What is AWS Lambda?

AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

### 2.Name some use cases for AWS Lambdas.

1. individual tasks run for a short time
2. each task is generally self-contained
3. there is a large difference between the lowest and highest levels in the workload of the application

### 3.Describe “serverless” to a non-technical friend.

The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions. AWS Lambda is a fully managed service that takes care of all the infrastructure for you. And so “serverless” doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of, so that you can focus on writing application code.

## CDN

### 1.What is a CDN?

A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

### 2.How does a CDN work with relation to the website visitor?

The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page. When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content. CDNs will also communicate with the originating server to deliver any content that has not been previously cached.

### 3.What are the benefits of employing a CDN?

Employing a CDN doesn’t only speed up the delivery of Internet content, it helps protect your website against certain forms of cyber attacks, such as Denial of Service attacks. It protects against these threats because CDNs allow for the handling of more traffic and withstanding hardware failure better than many origin servers.
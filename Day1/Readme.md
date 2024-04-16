Introduction to AWS

Let's learn how to create AWS account and fundamentals of cloud computing 

[Types of cloud computing](#types-of-cloud-computing)

what is cloud computing ?
- providing compute resources over internet is called cloud computing.

**Benefits of AWS**
- pay-per use payment model
- Instant scalability/go-global in minutes
- Reliable/redundant
- Highly secured
  

### Types of cloud computing

- Cloud computing types are divided into two types, they are 1. Service models 2. Deployment models
  
  Before going to know about them, let's know about virtualization first
<details>
<summary>Why do organizations and businesses use virtualization for cloud computing? </summary><br><b>

using virtualization increases the efficient use of hardware, which in turn lowers the cost of building, sustaining, and hosting computers in data centers as a cloud service. Virtualization products are therefore extremely important to businesses operating private or public clouds.
</b></details>


# Types of cloud computing {Based on service}
1. SAAS
2. PAAS
3. IAAS
   
**SAAS**:
- It is the simplest to use and the easiest to deploy
- With SAAS, Users have direct, on-demand access to shared applications and data over the internet.
- There is no software to install or configure - everything is available via web browser.
- EX: Microsoft office 365 and slack

**PAAS**:
- For users, who need more control and flexibility , PAAS is the solution
- With this service model, web developers and programmers can upload their content to pre-configured web servers, database servers, and application servers without having to install or maintain any of the servers’ applications or operating systems
- EX: Amazon S3, Amazon Route 53, AWS and GCP 
- with PAAS, we will get ready-to-go services that don't require the need to build or install anything from scratch.
- PAAS provides extra ability to build on top of the services by, for ex: Using API to integrate with another service and life-cycle management.

**IAAS**:
- For maximum control, IAAS can be used
- It gives access to a dedicated virtual or physical system that you manage and maintain yourself.
- IAAS Provides the greatest degree of flexibility and customization of the three cloud computing types.
- EX : Digital ocean
  
  ![on-premises](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/on-Premises.png)

  ![IAAS](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/IAAS.png)

  ![PAAS](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/PAAS.png)

  ![SAAS](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/SAAS.png)

![IAAS_analogy](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/IAAS_analogy.png)

![PAAS_analogy](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/PAAS_analogy.png)
![SAAS_analogy](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/SAAS_analogy.png)

![cloudcomputing stack](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/Types%20of%20Cloud%20Computing%20Stack.png)

# Types of cloud computing (Based on deployment Models)
- The world "deployment" used in computing circles, is usually refers to all the activities involved in making software or hardware available and ready for use : installation, configuration (setting up), testing, making changes, and then running
- Organizations choose among the different models based on their business goals, computing, networking and storage requirements and budget.

Basically there are 4 deployment models in cloud, they are

1. Private cloud
2. Public Cloud
3. Hybrid Cloud
4. Community cloud

![Cloud_deployment model](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/Cloud%20Deployment%20Model.png)

**Private clouds** are computing resources managed by a specific organization for internal business goals or objectives that typically reside on a company’s intranet or hosted data center. (It’s important to note here that a cloud doesn’t necessarily have to be on the internet.) 

**Public cloud** are usually managed by a third-party business or organization to offer computing resources to customers

**Community/hybrid cloud**

#### Global Infrastructure

 **Regions**
 - AWS Regions are geographically dispersed areas around the world that contain multiple Availability Zones. Customers can choose the region that best meets their requirements for factors such as data sovereignty, latency, and costs. 

  **Availability zones**
  - AWS Availability Zones (AZs) are distinct physical data center locations within a region, designed for high availability. They are interconnected with low-latency networking and offer redundant power, cooling, and networking. 

  **Edge Locations**
  - AWS Edge Locations are strategically positioned points of presence in the AWS network, optimized for low-latency content delivery. They are used to reduce latency for end-users by serving content from locations closer to them


All right, Let's Start the Cloud skill hunting by [creating AWS account](https://charanwrites.hashnode.dev/how-to-create-free-tier-aws-account).

See you on [Day2](https://github.com/charan-happy/AWS-Devops_Zero-to-Hero/tree/main/Day2)

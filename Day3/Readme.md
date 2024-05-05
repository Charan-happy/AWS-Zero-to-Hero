EC2 Instances

In EC2 Dashboard, we have 


<details><summary>
Instances section</summary>
instances <br> instance types <br> launch template <br> spot requests <br> saving plans <br> Reserved instances <br> dedicated hosts <br> capacity reservations
    </summary>
</details>
<details>
    <summary>
        images
    </summary>
    AMIS <br> AMI catalogue
    
</details>

<details>
    <summary>
        Elastic Block store
    </summary>
    volumes <br> snapshot <br> lifecycle manager<br>
</details>

<details>
    <summary>
        Network & Security
    </summary>
    security groups <br> elastic ips <br> placement groups <br> keypairs <br>network interfaces
</details>

<details>
    <summary>
        Load balancing
    </summary>
    LoadBalancers <br> target groups <br> trust stores 
</details>

<details>
    <summary>
        Autoscaling
    </summary>
    Autoscaling groups
</details>


# What is Amazon EC2?

    - Amazon Elastic Compute Cloud (Amazon EC2) provides on-demand, scalable computing capacity in the Amazon Web Services (AWS) Cloud. Using Amazon EC2 reduces hardware costs so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage
    - with Ec2 we can easily scale up or scaledown the capacity.
## [features](#features-1)

## [Get Started](#get-started-1)

## [Access Ec2](#access-ec2-1)

## [pricing](#pricing-1)



### features
- Amazon Ec2 has the following high-level features:
  
    <b><details><summary>Instances</summary><br><b>
  Virtual Servers</details>
    <details><summary>Amazon Machine images (AMI)</summary><br><b>Pre-configured templates for your instances that package the components you need for your server (including the os and additional software)</details>

    <details><summary>Instance Types</summary><br><b>Various configurations of CPU, memory, storage, networking capacity, and graphics hardware for your instances.</details>

    <details><summary>key pairs</summary><br><b>Secure login information for your instances. AWS stores the public key and you store the private key in a secure place.</details>

    <details><summary>Instance Store volumes</summary><br><b>Storage volumes for temporary data that is deleted when you stop, hibernate, or terminate your instance.</details>

    <details><summary>Amazon EBS Volumes</summary><br><b>Persistent storage volumes for your data using Amazon Elastic Block Store (Amazon EBS).</details>

    <details><summary>Regions, AZ, local zones, AWS Outposts, and wavelength Zones</summary><br><b>Multiple physical locations for your resources, such as instances and Amazon EBS volumes.</details>

    <details><summary>Security Groups</summary><br>
      A virtual firewall that allows you to specify the protocols, ports, and source IP ranges that can reach your instances, and the destination IP ranges to which your instances can connect.</details>

    <details><summary>Elastic IP addresses</summary><br><b>Static IPv4 addresses for dynamic cloud computing.</details>

    <details><summary>Tags</summary><br><b>Metadata that you can create and assign to your Amazon EC2 resources</details>

    <details><summary>Virtual Private Clouds (vpcs)</summary><br><b>Virtual networks you can create that are logically isolated from the rest of the AWS Cloud. You can optionally connect these virtual networks to your own network.</details>

### Get Started


### Related Services

    we can provision Amazon EC2 resources, such as instances and volumes, directly using Amazon EC2. In addition, you can provision EC2 resources using other AWS services, such as the following

    - Amazon EC2 Auto Scaling
       >  Helps ensure we have correct number of Amazon Ec2 instances available to handle the load for our application

    - AWS Cloud Formation 
      > Helps to model and setup our AWS resources using templates
    
    - AWS Elastic Beanstalk
      > Deploy and manage applications in the AWS Cloud without having to understand the underlying infrastructure

    - AWS OpsWorks
        > Automate how servers are configured, deployed, and managed across your Amazon EC2 instances using chef and puppet
    - EC2 Image Builder
      > Automate the creation, management, and deployment of customized, secure and up-to-date server images

    - AWS Launch wizard
      > size, configure and deploy AWS resources for third-party applications without having to manually identify and provision individual AWS resources    

### Access EC2

    we can create and manage our Amazon EC2 instances using the following interfaces :

<details><summary>Amazon EC2 Console</summary>
        
    > A simple web interface to create and manage Amazon EC2 instances and resources.
</details>
<details><summary>
AWS Command Line Interface
</summary>
    
    > Enables us to interact with AWS Services using commands in our command-line shell. It supported on windows, Mac and Linux
</details>

<details><summary>AWS Tools for Powershell</summary>

> A set of powershell modules that are built on the functionality exposed by the AWS SDK for .NET. The tools for powershell enable us to script operations on our 
            AWS resources from the powershell command line.
</details>

<details><summary>AWS cloudFormation
</summary>
    
    > Amazon EC2 supports creating resources using AWS Cloudformation. we create template in JSON or YAML format, that describes our AWS resources and AWS CloudFormation provisions and configures those resources for you. we can reuse your CloudFormation templates to provision the same resources multiple times, whether in the same Region and account or in multiple Regions and accounts
</details>

<details>
<summary>
Query API
</summary>
    > Amazon EC2 provides a Query API. These requests are HTTP or HTTPS requests that use the HTTP verbs GET or POST and a Query parameter named Action
</details>

<details><summary>
AWS SDKs
</summary>
    
    > If you prefer to build applications using language-specific APIs instead of submitting a request over HTTP or HTTPS, AWS provides libraries, sample code, tutorials, and other resources for software developers. These libraries provide basic functions that automate tasks such as cryptographically signing your requests, retrying requests, and handling error responses, making it easier for you to get started
</details>


### Pricing

Amazon EC2 provides the following pricing options:

    Free tier

    on-Demand Instances

    Savings-plans

    Reserved Instances

    Spot Instances

    Dedicated Hosts

    on-Demand capacity Reservations

    per-second billing


[Click Here to more about Amazon EC2](https://docs.aws.amazon.com/AWSEC2)

[Day4](https://github.com/charan-happy/AWS-Devops_Zero-to-Hero/tree/main/Day4)

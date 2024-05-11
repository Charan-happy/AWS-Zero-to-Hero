I AM [Identity Access Management]

Dashboard Walkthrough :

<details> <summary>Access management</summary>User groups <br> users <br> Roles <br> Policies <br> Identity Providers <br> Account Settings</details>

<details><summary>Access Reports</summary>Access Analyzer <br>-  Exeternal Access <br> - Unused access <br> - Analyser settings <br> Credential Report <br>Organization activity <br> Service control policies</details>
First, let's see what are the concepts that we need to learn in IAM Services in AWS.

# How IAM Works

# what is IAM ?
- IAM stands for Identity and Access Management
- AWS IAM is a webservice provided by AWS that helps you securely control access to AWS resources.
- With IAM we can centrally manage permissions that control which AWS resources users can access.
- We can Use IAM to control who is authenticated (signed in) and authorized(has permissions) to use resources.

# IAM Features
IAM gives the following features for us:
<details><summary><b>1. Shared access to your AWS account</summary><br><b>

    You can grant other people permission to administer and use resources in your AWS account without having to share your password or access key.
</details>

<details>
<summary>2. Granular permissions</summary><b>

    You can grant other people permission to administer and use resources in your AWS account without having to share your password or access key. EX: We might allow some users complete access to EC2, S3,Redshift etc. But, for other users, we can allow read-only permission to S3 buckets, only administrator access to some ec2 instances or acces to only billing information etc.
</details>
<details><summary>3. secure access to AWS resource for applications that run on Amazon EC2</summary> <br><b>

    You can use IAM features to securely provide credentials for applications that run on EC2 instances. These credentials provide permissions for your application to access other AWS resources. Examples include S3 buckets and DynamoDB tables.

</details>
<details>
<summary>
4. Multifactor Authentication(MFA)</summary><br><b>
    
    You can add two-factor authentication to your account and to individual users for extra security. With MFA you or your users must provide not only a password or access key to work with your account, but also a code from a specially configured device  
</details>
<details><summary>5. Identity federation</summary><br><>
    
    You can allow users who already have passwords elsewhere—for example, in your corporate network or with an internet identity provider—to get temporary access to your AWS account.
</details>
<details><summary>6. Identity information for assurance
</summary><br><b>


    If you use AWS CloudTrail, you receive log records that include information about those who made requests for resources in your account. That information is based on IAM identities.
</details>
<details><summary>
7. PCI DSS [Payment card industry Data security standard]Compilance</summary><br><b>
   
   
    IAM supports the processing, storage, and transmission of credit card data by a merchant or service provider, and has been validated as being compliant with Payment Card Industry (PCI) Data Security Standard (DSS).
</details>
<details><summary>
8. Integrated with Many AWS Services</summary><br><b> 


[List of services we can integrate with IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_aws-services-that-work-with-iam.html)
   </details>
<details><summary>
9.  Eventually consistent</summary><br><b>
    
    IAM, like many other AWS services, is eventually consistent. IAM achieves high availability by replicating data across multiple servers within Amazon's data centers around the world. If a request to change some data is successful, the change is committed and safely stored. However, the change must be replicated across IAM, which can take some time

    But, AWs itself recommends us to do not include such IAM changes in the critical, high-availability code paths of your application. Instead, make IAM changes in a separate initialization or setup routine that you run less frequently.
</details>

<details><summary>
10.     Free to use</summary><br><b>
    
        AWS IAM and AWS Security Token Service(AWS STS) are features of your AWS account offered at no additional charge. You are charged only when accessing other AWS services using Your IAM users or AWS STS temporary security credentials.

</details> </br>

Ways to Access IAM :

- **AWS Management console**

- **AWS Command line tools**

- **AWS SDKs**

- **IAM Query API**

# When do i Use IAM
<details><summary>1. When you are performing different job functions</summary><br><b>

    AWS Identity and Access Management is a core infrastructure service that provides the foundation for access control based on identities within AWS. You use IAM every time you access your AWS account.

    How you use IAM differs, depending on the work that you do in AWS.

        we can use IAM in 3 different ways as an user, 
        1. Service user 2. Service Administrator 3. IAM Administrator
</details>
<details><summary>2. When you are authorized to Access AWS Resources</summary><br><b>

    Authentication is how you sign in to AWS using your identity credentials. You must be authenticated (signed in to AWS) as the AWS account root user, as an IAM user, or by assuming an IAM role.

    You can sign in to AWS as a federated identity by using credentials provided through an identity source.

</details>
<details><summary>3. When you sign in as an IAM user</summary><br><b>
   
    An IAM user is an identity within your AWS account that has specific permissions for a single person or application. Where possible, we recommend relying on temporary credentials instead of creating IAM users who have long-term credentials such as passwords and access keys. However, if you have specific use cases that require long-term credentials with IAM users, AWS recommend that you rotate access keys.

    An IAM group is an identity that specifies a collection of IAM users. You can't sign in as a group. You can use groups to specify permissions for multiple users at a time. Groups make permissions easier to manage for large sets of users. For example, you could have a group named IAMAdmins and give that group permissions to administer IAM resources.

    Users are different from roles. A user is uniquely associated with one person or application, but a role is intended to be assumable by anyone who needs it. Users have permanent long-term credentials, but roles provide temporary credentials. 

</details>
<details><summary>4. When you assume an IAM Role</summary><br><b>

    An IAM role is an identity within your AWS account that has specific permissions. It is similar to an IAM user, but is not associated with a specific person. You can temporarily assume an IAM role in the AWS Management Console by switching roles. You can assume a role by calling an AWS CLI or AWS API operation or by using a custom URL

    IAM roles with temporary credentials are useful in the following situations:
        - Federated user access
        - Temporary IAM user permissions
        - Cross-account access
        - Cross-service access
            A service might do this using the calling principal's permissions,using a service role, or using a service-linked role. 
       - Applications running on Amazon EC2
</details>
<details><summary>5. When you Create Policies and permissions</summary><br><b>

    You grant permissions to a user by creating a policy, which is a document that lists the actions that a user can perform and the resources those actions can affect. Any actions or resources that are not explicitly allowed are denied by default. Policies can be created and attached to principals (users, groups of users, roles assumed by users, and resources).

    These policies are used with an IAM role:
        Trust policy : Defines which principals can assume the role, and under which conditions. A trust policy is a specific type of resource-based policy for IAM roles. A role can have only one trust policy.

        Identity-based policies (inline and managed) – These policies define the permissions that the user of the role is able to perform (or is denied from performing), and on which resources.
</details>


## How IAM Works

IAM provides the infrastructure necessary to control authentication and authorization for your AWS account. The IAM infrastructure is illustrated by the following diagram:

![how iam works](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/HOW-IAM-Works.png)

First, a human user or an application uses their sign-in credentials to authenticate with AWS. Authentication is provided by matching the sign-in credentials to a principal (an IAM user, federated user, IAM role, or application) trusted by the AWS account.

Next, a request is made to grant the principal access to resources. Access is granted in response to an authorization request. For example, when you first sign in to the console and are on the console Home page, you are not accessing a specific service. When you select a service, the request for authorization is sent to that service and it looks to see if your identity is on the list of authorized users, what policies are being enforced to control the level of access granted, and any other policies that might be in effect. Authorization requests can be made by principals within your AWS account or from another AWS account that you trust.

Once authorized, the principal can take action or perform operations on resources in your AWS account. For example, the principal could launch a new Amazon Elastic Compute Cloud instance, modify IAM group membership, or delete Amazon Simple Storage Service buckets.

# Basic Concepts

## Terms

- These IAM terms are commonly used when working with AWS:

IAM Resource
IAM resources are stored in IAM. You can add, edit, and remove them from IAM.

    user

    group

    role

    policy

    identity-provider object

IAM Entity

IAM resources that AWS uses for authentication. Entities can be specified as a Principal in a resource-based policy.

    user

    role

    IAM Identity

An IAM resource that can be authorized in policies to perform actions and to access resources. Identities include users, groups, and roles.

Principals

A person or application that uses the AWS account root user, an IAM user, or an IAM role to sign in and make requests to AWS. Principals include federated users and assumed roles.

Human users

Also known as human identities; the people, administrators, developers, operators, and consumers of your applications.

Workload

A collection of resources and code that delivers business value, such as an application or backend process. Can include applications, operational tools, and components.

![IAM Terms](https://github.com/Charan-happy/AWS-Devops_Zero-to-Hero/blob/main/Images/iam-terms.png)

# users in AWS

# Permissions and policies in IAM

# What is ABAC
    
    Attribute-based access control (ABAC) is an authorization strategy that defines permissions based on attributes. In AWS, these attributes are called tags. 
    
    You can attach tags to IAM resources, including IAM entities (users or roles) and to AWS resources. You can create a single ABAC policy or small set of policies for your IAM principals. These ABAC policies can be designed to allow operations when the principal's tag matches the resource tag. ABAC is helpful in environments that are growing rapidly and helps with situations where policy management becomes cumbersome.

ABAC provides the following advantages over the traditional RBAC model:

    ABAC permissions scale with innovation.

    ABAC requires fewer policies

    Using ABAC, teams can change and grow quickly

    Granular permissions are possible using ABAC

    Use employee attributes from your corporate directory with ABAC

[Let's get our hands Dirty by doing IAM practicles in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html#getting-started-prereqs)    


[Additional in_depth Reading about IAM](https://docs.aws.amazon.com/IAM)

Now we have our permissions Ready to start something in AWS cloud, go ahead with [Day3](https://github.com/charan-happy/AWS-Devops_Zero-to-Hero/tree/main/Day3)

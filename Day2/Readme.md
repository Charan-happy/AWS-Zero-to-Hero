I AM [Identity Access Management]

First, let's see what are the concepts that we need to learn in IAM Services in AWS.


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











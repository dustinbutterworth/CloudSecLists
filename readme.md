### About CloudSecLists
CloudSecLists is a collection of tools that are useful for securing a cloud environment. This list will start off fairly simple, then once I get enough things added I will separate the tools into Blue Team, Red Team, and maybe Purple Team.  I will try to come up with a system to let the user knows if they are useful for AWS, Azure, GCP, etc...

## AWS  

### General
[AWS Well Architected Labs: Security](https://www.wellarchitectedlabs.com/security/) - The security labs are documentation and code in the format of hands-on labs to help you learn, measure, and build using architectural best practices.  

### Enumeration
[Metasploit: enum_iam](https://www.rapid7.com/db/modules/auxiliary/cloud/aws/enum_iam/) - Provided AWS credentials, this module will call the authenticated API of Amazon Web Services to list all IAM credentials associated with the account  
[Metasploit: enum_ec2](https://www.rapid7.com/db/modules/auxiliary/cloud/aws/enum_ec2/) - Provided AWS credentials, this module will call the authenticated API of Amazon Web Services to list all EC2 instances associated with the account  
[Metasploit: enum_s3](https://www.rapid7.com/db/modules/auxiliary/cloud/aws/enum_s3/) - Provided AWS credentials, this module will call the authenticated API of Amazon Web Services to list all S3 buckets associated with the account  

### S3
[Grayhat Warfare Public Bucket Search](https://buckets.grayhatwarfare.com/) - Search engine for finding open S3 buckets.  
[S3Scanner](https://github.com/sa7mon/S3Scanner) - A tool to find open S3 buckets and dump their contents  
[S3-Inspector](https://github.com/clario-tech/s3-inspector) - Checks all your buckets for public access  
[AWS Extender](https://github.com/VirtueSecurity/aws-extender) - This Burp Suite extension can identify and test S3 buckets as well as Google Storage buckets and Azure Storage containers for common misconfiguration issues using the boto/boto3 SDK library.  
[minio](https://github.com/minio/minio) - Set up a local S3 type lab you can test your scripts against. See https://medium.com/@jonathanchelmus/creating-an-s3-lab-on-an-ec2-instance-95ffd8ac6c1  
[Recon-Public-Buckets](https://github.com/Moos1e/Recon-Public-Buckets) - Example of using bash + aws cli against a list of buckets to see if you have public buckets in your environment.  

### Cloudformation
[cfn_nag](https://github.com/stelligent/cfn_nag) - Cloudformation template scanner. DevSecOps. My favorite of the Open Source ones.  
[checkov](https://github.com/bridgecrewio/checkov) - Cloudformation template scanner. DevSecOps.

### Lambda
[LambdaGuard](https://github.com/Skyscanner/LambdaGuard) - Audit and scan Lambda services  

### Informational Resources
[Python, Boto3, and AWS S3: Demystified](https://realpython.com/python-boto3-aws-s3) - Work with S3 via Python Boto3 module.  

### Attribution
Dustin Butterworth - dustin.butterworth@protonmail.com  

### Resources   
[AWS Penetration Testing by Jonathan Helmus](https://www.amazon.com/AWS-Penetration-Testing-Beginners-Metasploit/dp/1839216921) - Many tools from this list gathered from this book. Highly recommend buying it!  

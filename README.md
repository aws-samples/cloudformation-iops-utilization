## Visualizing usage of Provisioned IOPS volumes on Amazon EBS for analysis
This code is part of a blog post

## Prerequisites
For this tutorial, you should have the following prerequisites:
* An AWS account
* AWS resources: Provisioned IOPS volumes
* AWS services: Amazon S3, AWS CloudFormation, Amazon CloudWatch, AWS Identity and Access Management (IAM), and AWS Lambda

##  Code Overview
CloudFormation template deploys a Lambda function. The function, once invoked, captures CloudWatch metrics which are enhanced and transformed for IOPS calculations. The function generates a unique CSV file in S3 containing metrics for the last 7 days for each io1/io2 scanned volumes and can be parameterized for a larger time span. With minimal development effort, the script can be changed to capture metrics that might be relevant to other EBS volume types as well.

##  Main Files
* EBSAnalyzer.yaml -> CloudFormation template that deploy the code(index.zip)
* index.zip -> Zipped file containing the lambda function code written in Python.


##  Installation instrutions
Detailed instrutions can be found in the blog post.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.


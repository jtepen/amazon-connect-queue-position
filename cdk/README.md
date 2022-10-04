# Amazon Connect Queue Position Stack

## Prerequisites

An S3 bucket is required for the deployment of the Lambda function.

## Setup

https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html

1. Install [NodeJS](https://nodejs.org/en/download/)
2. Install [Python](https://www.python.org/downloads/)
3. Install the aws-cdk-lib library: ```python -m pip install aws-cdk-lib```
4. Install the AWS CDK Toolkit: ```npm install -g aws-cdk```

## Resources

1. Lambda Function + Role & Policy
2. DynamoDB Table

## Deploy

Use the following command to deploy the Stack, or use the pre-generated CloudFormation Template.

```
cdk deploy -c account_id=x -c region=ap-southeast-2 \
--parameters deploymentBucket=deployment_bucket \ 
--parameters lambdaKey=lambda.zip \
--parameters amazonConnectId=xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
```

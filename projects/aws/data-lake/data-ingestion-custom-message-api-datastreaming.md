# Data Ingestion - Real Time mock data stream with custom API

## Purpose
Simulate custom message to create a mock real-time data streaming API

### Tasks
- Create S3 bucket structure
- Create a service role for AWS Glue . [Click here](https://github.com/e2eSolutionArchitect/scripts/blob/main/aws/iam/policies/aws-policy-glue-crawler.json)
- Create AWS Lambda function with Python runtime for simulating JSON message. [Click here](https://github.com/e2eSolutionArchitect/scripts/blob/main/aws/lambda/lambda-generate-twitter-message-stream.py)
- Create Amazon API Gateway REST API and link trigger with above AWS Lambda function
- Write a python script to invoke the REST API iteratively
- Test the custom message API

![image](https://user-images.githubusercontent.com/62712515/224165983-cf5b2e2a-7f3c-4cf4-9412-0539d9fab64d.png)


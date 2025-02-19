# How to build a serverless marketing email application
*Some personal notes on how to build a serverless marketing email application on AWS.*

## Services involved: 
  - AWS simple email service (SES)
  - AWS lambda
  - S3
  - Amazon eventbridge
  - IAM

## Steps
1. Create a S3 bucket for email templates and contacts
2. Set up SES for sender and receiver emails
3. Create a lambda function for email logic & test
4. Add permission for lambda: configuration - permissions - role name (enter IAM) -  add permission - add policy
5. Set up trigger in eventbridge


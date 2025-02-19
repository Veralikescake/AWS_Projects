# WildRydes Web App

*Some personal notes on how to create a web app on AWS.* 

*Relevant codes: https://github.com/Veralikescake/wildrydes-site*

## Services involved: 
  - Amplify
  - AWS lambda
  - Cognito
  - AWS API Gateway
  - IAM
  - DynamoDB
  - Github

## Steps
1. Create a new repo on github to store codes.
2. Create & host an app in Amplify with codes in the new repo.
3. Set up user pool in Cognito for user authentication, and update config.js to link up the app with the user pool.
4. Create a new table in DynamoDB to store rides info.
5. Create a new Lambda function for execute ride requests (replace table name in the code).
    - Before create the Lambda function, set up a new role in IAM to give it DynamoDB write access.
6. Use API gateway to invoke the ride request function. 
    - To hook it up with the cognito, create an authorizer in it.
    - Create a new resourse, enable CORS, and add a POST methodm with authorization
    - Deploy the API, and copy the invoke url to the config doc.


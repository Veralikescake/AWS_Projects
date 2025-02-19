# Card match game with continous deployment pipeline

*Some personal notes on how to create a game with continous deployment pipeline on AWS.*


*Relevant codes: https://github.com/Veralikescake/codepipeline-s3-game*

## Services involved: 
  - CodePipeline
  - S3
  - Github

## Steps
1. Create a S3 bucket.
   - Under property, enable "static website hosting"
   - Under permission, edit bucket policy to be publicly accessible ([Policy link](./Bucket%20Policy.docx))
2. Set up code pipeline between github and S3.
   - Only v2 can be created in the console now.
3. Deployment succcessful. Make small changes to the code in github to test continuous deployment.
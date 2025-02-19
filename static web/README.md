## Host a Static Web on AWS S3
*Some personal notes on how to host a website using S3.*
1. **Bucket crreation:** Navigate to AWS S3, create a bucket, and edit 'Property' - 'Static website hosting' - 'Enable'
2. **Public access:** Public access is denied from buckets y default, navigate to 'Permission' and enable access.
3. **Update Policy:** Replace 'bucket-name' with the actual ARN of your bucket.
4. **Upload Objects:** Upload index.html and relevant files to 'Objects'
5. Here goes the website! http://veraawsbucket.s3-website.us-east-2.amazonaws.com
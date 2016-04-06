# lambda-s3_access_logs_to_cloudwatch
Consumes S3 Bucket Access logs and pushes them to CloudWatch

## Setup
```
git clone git@github.com:aegixx/lambda-s3_access_logs_to_cloudwatch.git
cd lambda-s3_access_logs_to_cloudwatch
npm install
```

## AWS Lambda
(http://docs.aws.amazon.com/lambda/latest/dg/getting-started.html)
```
# Zip the deployment package
zip -rq /tmp/lambda-s3_access_logs_to_cloudwatch.zip *
# Upload the deployment package to AWS Lambda or use CLI
aws lambda create-function --function-name "lambda-s3_access_logs_to_cloudwatch" --runtime nodejs --role <YOUR_LAMBDA_IAM_ROLE> --handler index.handler
```

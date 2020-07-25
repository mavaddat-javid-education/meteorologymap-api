# Chasing Weather API

API for an app to provide trip-planning based on geospatial weather forecasting.

## Deployment

We deploy the application using the AWS Serverless Application Model \(AWS SAM\) &mdash; an open\-source framework for building [serverless applications](https://aws.amazon.com/serverless/) on AWS\.

### Pre-requisites

- [Locally set up AWS Environment](https://github.com/awsdocs/aws-sam-developer-guide/blob/master/doc_source/serverless-getting-started.md)

### Overview

`git clone` <https://github.com/mavaddat-javid-education/meteorologymap-api.git> ➡ `sam build` ➡ `sam package` ➡ `sam deploy`

### Step 1

```bash
sam build
```

### Step 2

```bash
sam package --s3-bucket [s3-bucket-name] --output-template-file output.yaml
```

### Initial deployment

```bash
sam deploy --template-file output.yaml --stack-name [stack-name] --capabilities CAPABILITY_IAM
```

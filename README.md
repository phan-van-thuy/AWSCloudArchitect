## Udacity AWS Cloud Architect ##
## Deployt VPC Using CloudFormation
- Source config on folder cloudformation/vpc.yaml
## Using Primary VPC
# Command Create 
aws cloudformation deploy --template-file .\vpc.yaml --stack-name vpc-primary --tags project=udapeople --capabilities CAPABILITY_NAMED_IAM --region us-east-1  --parameter-overrides VpcName=Primary
## Using Secondary VPC
# Command Create 
aws cloudformation deploy --template-file .\vpc.yaml --stack-name vpc-secondary --tags project=udapeople --capabilities CAPABILITY_NAMED_IAM --region us-west-2  --parameter-overrides VpcName=Secondary

## My link github 
- https://github.com/phan-van-thuy/AWSCloudArchitect

##### Udacity AWS Cloud Architect  #####

## Folder structure

| File | Description |
| ---- | ----------- |
| `cloudformation` | Source Build VPC infrastructure as code |
| `cloudformation/pvc.yaml` | Cloudformation code |
| `s3` | Source application |


## Link s3 project 
http://thuypv.s3-website-us-east-1.amazonaws.com/
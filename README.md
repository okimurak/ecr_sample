# ECR Sample

Use terraform_sample resource

## Require

- Docker
- AWS-Cli

## Build

```
docker build -t <Your AWS Account Id>.dkr.ecr.${YOUR_AWS_REGION}.amazonaws.com/example .
```


## Upload

```
 $(aws ecr get-login --no-include-email --region <YOUR_AWS_REGION>)
docker push <Your AWS Account Id>.dkr.ecr.${YOUR_AWS_REGION}.amazonaws.com/example
```
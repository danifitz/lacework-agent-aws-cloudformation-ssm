# Lacework CloudFormation SSM Agent Deployment

Before you run this template you need to [setup AWS Systems Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-quick-setup.html) so that your EC2 instances have the necessary IAM role attached.

## Prerequisites

1. SSM enabled for Node Management. EC2 instances need to have `amazon-ssm-agent` installed and have an instance role/profile attached with the `AmazonSSMManagedInstanceCore`
policy.
2. Additionally - for the Lacework agent access token to be pulled from AWS Secrets Manager, the instance profile/role needs to have `secretsmanager:GetSecretValue` IAM permission.

## Usage

This template can be deployed in a single AWS account or across an OU/Org via CloudFormation stacksets.

### Single Account

TODO

### AWS OU/Org

via stacksets. TODO
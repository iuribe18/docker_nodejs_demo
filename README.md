# Providing access to AWS from GitHub Actions using Open ID Connect
# Resource:
https://medium.com/schmiedeone/providing-access-to-aws-from-github-actions-using-open-id-connect-bf3daa3c9cd3
1. Create an identity provider
Provider URL:https://token.actions.githubusercontent.com
Audience: sts.amazonaws.com
Output ARN: arn:aws:iam::735948513526:oidc-provider/token.actions.githubusercontent.com

2. Create a rol Custom trust Policy
Add policy: AmazonEC2ContainerRegistryFullAccess, AmazonECS_FullAccess
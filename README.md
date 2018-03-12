# AWS DspaceOrchestration


[![Launch Stack](https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=dspacesample&templateURL=https://s3-eu-west-1.amazonaws.com/puppet-serverless/NestedStacks2/dspace_project_staging_cloudformation.template)

This AWS CloudFormation templates create a full infrastructure for DspaceDirect application deployment, the following has a summary of all the the template does:

This AWS CloudFormation template creates the full Dspace infrastracture which includes the following:

  - a dedicated [Amazon Virtual Private Cloud](https://aws.amazon.com/vpc) (VPC) for the stack components, with 3 public subnets;
  - One Internet Gateway;
  - a Route Table;
  - 3 Mount Targets;
  - Elastic File System.
  - 3 Auto Scaling Groups each with 3 Launch Configurations
  - One Application Load Balancer
  - 3 Security Groups
  - Route 53 Record Sets
  - Aurora Postgres RDS
  - Instance type t2.xlarge
  - Db class r4.large for the aurora database
  - One s3 bucket for the manifest files
  - 6 Target Groups
  - Two Lambda Functions for the computation
  
# General Architecture 
![alt text](https://github.com/dspaceproject/DspaceOrchestration/blob/master/files/image.png)

# init-templates

* Description

These are the cloud formation templates you can choose from to start a ha-cms environment. Once a template is started it will create the admin level infrastructure and download relevant packages from GitHub to configure the application layer and any other AWS components that couldn't be configured by cloudformation directly

* Prerequisites

1. Ensure you have an AWS account with root access or sufficient admin access
2. Create an IAM Role with Admin Access (will only be used during initialization)
3. Create a keypair and ensure the private key is saved. One lost you can't get it back and you need it to access the utility in the event you want to get to the backend of the systems

* Installation

Go to CloudFormation and when creating a stack, choose this as the template.

For the stack name, recommended not to have - as it's used as a separator in the naming standards. For all other parameters, the template will advise you what to enter

* Usage

Please allow up to 20 minutes for the stack to complete. Note that even when it says the stack is finished, the stack needs to under go an update after.

One stack has finished updating, go to the load balancer section in EC2 and enter the default load balancer DNS into your browser to access the admin server
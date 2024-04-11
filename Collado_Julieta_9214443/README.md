# Installation Manual: Hosting a Simple HTML Page on AWS using Terraform

## Introduction

Welcome to the installation manual for hosting a simple HTML page on AWS using Terraform. This guide will walk you through the process of deploying a basic website that displays "Hello Professor!" on the screen.

## Prerequisites

Before you begin, please make sure you comply with:

- An AWS account with appropriate permissions to create and manage resources.
- Terraform installed on your local machine. You can download terraform from terraform.io and follow the installation instructions for your operating system.

## AWS Setup

If you don't already have an AWS account, you will need to sign up for one at aws.amazon.com . Once you have an account, make sure you have access credentials (access key ID and secret access key) with the necessary permisions for creating resources.

## Terraform Installation

Follow these steps to install Terraform on your local machine:

1. Download the appropiate Terraform binary for your operating system from terraform.io/downloads.html .
2. Extract the downloaded archive to a directory on your machine.
3. Add the directory containing the Terraform binary to your system's PATH environment variable.

## Configuration Files

In your projct directory, you will find the following Terraform configuration files:

- `main.tf`: Defines the AWS infrastructure components (CloudFront, Lambda, S3 bucket).
- `lambda_function.zip`: Contains the Lambda function code.

You may need to customize these files to match your specific requirements.

## Deployment Process

Follow these steps to deploy the infrastructure and host the HTML page on AWS: 

1. Open a terminal and navigate to your project directory.
2. Run `terraform init` to initialize the Terraform configuration.
3. Run `terraform plan` to review the excecution plan and ensure everything looks correct.
4. Run `terraform apply` to apply the changes and deploy the infrastructure.
5. Wait for Terraform to complete the deployment process. Once finished, it will display the URL of your website.

## Testing and Verification

To verify that your website is hosted successfully, open a web browser and navigate to the URL provided by Terraform. You should see a webpage displaying "Hello Professor!".

## Cleanup

After you are done testing, remember to clean up the resources to avoid incurring unnecessary costs:

1. Run `terraform destroy` to tear down the infrastructure and remove the deployed resources.
2. Confirm the action when prompted.

## Support and Resources

For additional support or assistance, refer to the Terraform documentation at terraform.io/docs or the AWS documentation at docs.aws.amazon.com

## Conclusion

Congrats! You have successfully deployed a simple HTML page on AWS using Terraform. 

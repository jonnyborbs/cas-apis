# VMware Cloud Automation Services Postman Collection

This is a collection of REST API calls for use with Postman. We have included the following items:
* The actual Postman collection
* A Postman environment JSON

Import both of these into Postman to get started. You will need to obtin a Cloud Services Portal API Token for your org in order to authenticate. This token can be obtained by logging in to Cloud Services and selecting "My Account" from the dropdown at the right hand side.

## Required Variables
The environment JSON includes several variables that must be completed prior to executing any of the calls, including:
* refreshToken: Where you should input the API token obtained from Cloud Services
* url-home: The base URL of your Cloud Automation install. For Cloud Services, this is pre-filled.
* azureSubscriptionId: Your Azure subscription ID
* azureTenantId: Your Azure Tenant ID
* azurePrivateKeyId: The Application ID used to authenticate to your Azure account
* azurePrivateKey: The secret key for your Azure Application
* azureRegion: The regions you want to use for Azure
* awsPrivateKeyId: Your AWS Private Key ID (IAM Key)
* awsPrivateKeyId: Your AWS secret key
* awsRegion: The regions you want to use for AWS
* projectAdmins: The users (identified by email address) you want to be Project Administrators
* projectUsers: The users (identified by email address) you want to be Project Users

This API collection is a sample of what can be done with the Cloud Automation stack very simply. We will be providing updates to these files to include things like Day 2 Actions, object deletions, and more. 

## Usage
The "First Time Configuration" section of the collection is designed to be run end-to-end as a complete use case, executed in order of the numbered calls. Execute the **01 - Login** function first.

Note that the call **29 - Create Blueprint** requires the escaping of your blueprint YAML in order to be submitted. You can use a free JSON escape tool such as https://www.freeformatter.com/json-escape.html to do this easily.

## Contributions
Please feel free to submit pull requests or issues to this repository so we can monitor and update. Your changes are welcome as are your ideas. If you want additional information about the APIs directly, including links to the Swagger UI specs for them to aid in your development, please see https://blogs.vmware.com/management/2018/11/cloud-automation-services-api-first.html

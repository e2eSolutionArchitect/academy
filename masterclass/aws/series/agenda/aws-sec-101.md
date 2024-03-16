## :memo: AWS Security Session 01
- Session Code: [AWS-SEC-101](https://github.com/e2eSolutionArchitect/academy/blob/main/masterclass/aws/series/agenda/aws-sec-101.md)
- Description: AWS IAM Strategy
------------
***Prerequisites***
- AWS fundamental understanding
------------
:calendar: ***Schedule***

- Session type: Hybrid ( Classroom & Online ) <br>
- Registration link [click here](#) <br>
- Venue or Meeting details will be shared with registered candidates only
------------
***Agenda***
- AWS Organization
- - Root Account
  - OU & BU Accounts and Account hierarchy 
- AWS IAM use case
- Security best practices and use cases in AWS Identity and Access Management
- Security best practices in IAM
- Root user best practices for your AWS account 
- IAM Identity Center
- Business use cases for IAM
- Permission Boundary

------------
## Workshop

***AWS Organization***
- Create a BU Account

***IAM Roles & Policy***
- - Initial setup of a StartUp company 'DailyFresh'. Setup Administrative access to provision and manage AWS resources
  - Create three groups ( Admin, Manager, Developer)
  - Create Roles for ( Admin, Manager, Developer )
  -   - Admin should have system administrative access
      - Manager should have Billing access
      - The developer should have create and manage access to AWS resources
  - Create a policy that will allow the creation of selective serverless services ( dynamodb, EMR serverless, state function, etc.) for your AWS Account.
  - Create users ( Admin, Manager, Developer )
  - - IAM actions must have role/policy name starting with 'App_'
    - IAM role/policy actions should be restricted to specific AWS Accounts only
  - The new developer joined 'DailyFresh' IT department for AWS Cloud development. Please create a role for the Developer group, create and assign a policy allowing any developer to start creating and managing resources.
 
***Permission Boundary***
- The policy should not allow 'iam:*' action

***Service Control Policy (SCP)***
- Setup a SCP which will restrict any user ( except Admin user ) to create EC2 instances other than ( t2 and t3 series )

------------
***Next session agenda*** [click here](https://github.com/e2eSolutionArchitect/academy/blob/main/masterclass/aws/series/agenda/aws-sec-102.md)
------------
:star: AWS Workshop full list [here](https://github.com/e2eSolutionArchitect/academy/tree/main/masterclass/aws/series)

:writing_hand:  Please feel free to drop a note to e2eSolutionArchitect@gmail.com for any queries.

## :memo: IAM Session 01 
- Session Code: Azure-IAM-101
------------
***Prerequisites***
- Azure fundamental understanding
------------
:calendar: ***Schedule***

- Session type: Hybrid ( Classroom & Online ) <br>
- Registration link [click here](#) <br>
- Venue or Meeting details will be shared with registered candidates only
------------
***Agenda***
- Azure Organization
- - Root Account
  - OU & BU Accounts and Account hierarchy 
- Azure IAM [use case](#)
- Security best practices and use cases in Azure Identity and Access Management [click here](#)
- Security best practices in IAM
- Root user best practices for your Azure account - [click here](#)
- Business use cases for IAM
- Permission Boundary

 
## Workshop

***Azure Organization***
- Create a BU Account

***IAM Roles & Policy***
- - Initial setup of a StartUp company 'DailyFresh'. Setup Administrative access to provision and manage Azure resources
  - Create three groups ( Admin, Manager, Developer)
  - Create Roles for ( Admin, Manager, Developer )
  -   - Admin should have system administrative access
      - Manager should have Billing access
      - The developer should have create and manage access to Azure resources
  - Create a policy that will allow the creation of selective serverless services for your Azure Account.
  - Create users ( Admin, Manager, Developer )
  - - IAM actions must have role/policy name starting with 'App_'
    - IAM role/policy actions should be restricted to specific Azure Accounts only
  - The new developer joined 'DailyFresh' IT department for Azure Cloud development. Please create a role for the Developer group, and create and assign a policy allowing any developer to start creating and managing resources.
 
***Permission Boundary***
- The policy should not allow 'iam:*' action

***Service Control Policy (SCP)***
- Setup a SCP which will restrict any user ( except Admin user ) to create EC2 instances other than ( t2 and t3 series )

***Next session agenda*** [click here](https://github.com/e2eSolutionArchitect/academy/blob/main/masterclass/azure/series/agenda/session02.md)

:star: Azure Workshop full list [here](https://github.com/e2eSolutionArchitect/academy/tree/main/masterclass/azure/series)

:writing_hand:  Please feel free to drop a note to e2eSolutionArchitect@gmail.com for any queries.

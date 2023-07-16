## Project name: Small Business IT infrastructure setup in Azure Cloud

|   |   |
|---|---|
|  ***Description*** |  As a Cloud Engineer, you are assigned to a task to set up the required infrastructure for a Small Business in Azure Cloud. | 
| ***Business Case***  |  A Small Business Grocery shop 'DailyFresh' is new in town. As the name says, they deliver fresh vegetables to doorsteps based on the order they receive through their website. Every morning the traffic is expected to be very high (users more than 1000) for grocery orders. afternoon it is expected less than 100 visitors on the website<br> The owner of the business has hired you as Cloud Engineer to set up the necessary IT infrastructure in Cloud to run this business |
|  ***Regulatory Guidelines*** | <li> All infrastructure must be in Canada region only <li> Data should not be stored outside of Canada |
|  ***Requirement*** | ***Setup Organization*** <br> <li> Setup Organization hierarchy, Tenants, Management Group, Subscription. <li> Create two Users. One for application development. Another for managing Billing, Assign Roles, Enabling MFA for every user <br><br> ***Setup Policy*** <br> <li> User password must be alphanumeric with minimum 15 max 25 lengths <li> Password Should be changed in every 90 days <li> Password should not match last 5 passwords <li> No user should be able to log in without MFA <li> Every resource must have tags project, costcenter, createdby <li> Every resource must have these mandatory tags attached. projectname,createdfor,createdby,createdon,resourcename,costcenter  <br><br> ***Budget*** <li> Monthly budget should not exceed $20 <li> It should alert when 80% of the budget is reached  <br><br> ***Infrastructure*** <li> Create a custom vnets of CIDR 192.168.0.0/16 <li> Create two subnets in  vnet by equally diving the ip range <li> Create azureBastionHost in one subnet <li> Create a Linux VM in another subnet <li> Create a security group which will allow SSH access from bastion host only. and HTTP from public internet <li> Install httpd in VM <li> Create index.html and deploy in Apache webserver <li> Setup autoscaling. It should increase instance +1 when CPU usage goes more than 70%. <li> Create a load balancer to balance the traffic between VMs  <br><br>***Deploy Apps*** <br> <li> Setup CICD process to deploy a spring-boot application in AKS cluster <li> Deploy AngularApp (DailyFresh) in Azure cloud <br><br> ***Monitoring and Observability*** <li> Create a dashboard to show Network In and Out traffic trend <li> CPU utilization <li> No of storage accounts <li> No of VMs <br><br> ***Backup*** <li> Create backup of the VM in snapshot in daily frequency. <li> Keep last 2 backups only|
| ***DevSecOps***  |  ***Build*** <br> <li> Build and Create Image of a SpringBoot microservice <li> Store image in Azure Artifact <li> Provision and Deploy an AKS cluster  <br> ***Deploy*** <br><li> Deploy the app in AKS cluster <br> CI & CD <br><li> Setup Azure DevOps platform <li> Create Azure repo <li> Create Pipeline to deploy app in AKS cluster <br> ***Add Extension*** <br><li> Add extension in Pipeline <br> ***Set Security in DevOps*** <br><li> Setup Automated Static and Dynamic Testing <li> Setup Software Composition Analysis |
| ***Validation***  |  <li> Browse the load balancer url (or if the custom domain is mapped) and it should access the html content as a webpage. <li> Make minor changes in index.html. <li> Test REST service through Postman tool <li> Verify Angular app by url in browser|
| ***Given***  |  Create an html file named 'index.html' with content > ``` <h1> Happy learning with e2e Solution Architect </h1>  ```. Code for Angular app and microservice in GitHub repo  |
| ***Cost***  |  <li> This project WILL INCUR COST for purchasing a domain as well as the Azure services you plan to use. <li> You can use your existing personal domain (if any)|
| ***Pre-requisites***  |  <li> Azure portal access to implement the solution in your own Azure account <li> (Optional) A domain registered and available for use in this project  |
| ***Artifacts to be submitted***  |  <li> Solution Design (only two slides ppt format)  <li> ARM template/Terraform project in your GitHub public repository <li> A step-by-step clear documentation with screenshot in Markdown file. '.md' file for project documentation  <li> A max 5 minutes screen recording to show your implementation and testing. |
| ***Collaborate***  |  <li> Join the ***Slack** channel [here](https://talentdevelop-u8d3237.slack.com/archives/C04KCD5HPC1), collaborate with others to create a great solution <li>  |
| *** ***  |  ***You are most welcome to enhance the project with more detail and wide capabilities*** |


## Team

|   |   |
|---|---|
|  ***Team*** |  This project can be done in a Team. The team will be formed with a mix of expertise | 
|  ***Cloud Governance Team (CG)*** |  ***Roles & Responsibility*** <br><li> Create Subscription, Management Group and perform RBAC <li> Setup billing and budget |
|  ***Cloud Security Team (CS)*** |  ***Roles & Responsibility*** <br><li> Create Users, Role. <li> Define and setup organizational policy and standard <li> Define cloud security constructs like VNET, Subnet, Security Groups, WAF, etc |
|  ***Cloud Infrastructure Team (CI)*** |  ***Roles & Responsibility*** <br><li> Provision cloud resources, setup and configure | 
|  ***Cloud DevSecOps Team (DSO)*** |  ***Roles & Responsibility*** <br><li>  Automate Build, Deploy, Testing & Monitoring of any app. Setup security practice throughout the Continuous Integration & Continuous Deployment |
|  ***Cloud Monitoring Team (CM)*** |  ***Roles & Responsibility*** <br><li> Create Subscription, Management Group and perform RBAC<li> Setup billing and budget |
|  ***Cloud Application Developer Team (AD)*** |  ***Roles & Responsibility*** <br><li> Develop cloud-compatible web app in Angular/React or Springboot |
| *** ***  |  *** *** |


## Assignments

|  ***Team*** |  ***Area*** |  ***Tasks*** | *** *** |
|---|---|---| --- |
|  ***Cloud Governance Team (CG)*** | ***Governance***  | <li> Create TWO Subscriptions, ONE Management Group <li> Setup billing and budget <li> Define organization standards in plain text. The security team will implement these as Azure Policy | <li> Billing for Non-prod and prod should be separate|
|  ***Cloud Security Team (CS)*** | ***Security***  | <li>  Create one user for each team-role with least-required priviledge. Assign Roles, Enable MFA for every user <li> Setup organization policy mentioned by Governance team <li> Setup security policy for network hardening | |
| *** ***  |  *** *** |  *** *** | *** *** |

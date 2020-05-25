## AWS Lambda ##
***AWS Lambda*** is the service which computes the code without using server. It is said to be server-less computing.
- AWS Lambda is a compute service that let you run code without provisioning and managing the servers.
- With AWS Lambda you can run code for virtually any type of application or backend service or with zero administration.
(Here zero administartion means that all the things like who will run the code, maintenance, update and everything all will managed by AWS)
- AWS Lambda manages all the administration it manages: 
  - Provisioning and capacity of comute fleet that offers a balance of memory, CPU, network and other resources.
  - Server and OS maintenance
  - High availability and auto-scaling
  - Monitoring fleet health.
  - Applying security patches
  - Deploy your code.
  - Monitoring and logging your lambda function
- AWS Lambda executes your code only when needed and scales automatically from a few request per day to thousands per second.
(AWS runs your code only when it needed to run and we set trigger to tell AWS to run the code)
- You pay only for the compute time you consume and no charge when code is not executing.
- All you need to do is supply your code in form of one or more lambda functions to AWS Lambda in one of the language.
  - Node JS
  - Java
  - PowerShell
  - C#
  - Ruby
  - Python
  - Golang
  and the service will run on your behalf.
- Typically the lifecycle for AWS Lambda based application includes:
  - Authoring Code
  - Code deployed into AWS Lambda
  - Monitoring and troubleshooting
- In Lambda we can not enter to our Instance, we can not customise it, neither we can not change OS of our lambda and more.
- If you want to your own compute then you need to choose EC2 or Elastic Beanstalk.

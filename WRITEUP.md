# Write-up Template
### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- Cost:
  + Azure App service : Has lower cost than a virtual machine. App service also has built-in load balancers that help save infrastructure costs. App service is generally more cost-effective, it do not require control over the infrastructure. It provides a managed environment with predictable pricing and integrated features that simplify development, and scaling.
  + Virtual machine : Has higher cost than Azure App service because you have to manage and pay for virtual machines, underlying network resources and storage. So VM has greater flexibility and control, making them suitable for applications with specific infrastructure requirements or legacy systems that cannot be easily migrated to a PaaS environment. 

- Scalability:
  + Azure App service : I can easily increases or decreases resources allocated to my App service, such as the amount of vCPUs or RAM, by changing the App service pricing tier, auto-scaling and load balancing are integrated and managed by Azure. With Auto scaling App service can automatically scale the number of instances based on a schedule or metrics like CPU, memory or HTTP queue length. You have horizontal scaling (increase or decrease the number of instances) or vertical scaling (change the pricing tier to get more resources). 
  + Virtual machine : With VMs I can have greater control over the underlying infrastructure, allowing for custom configurations and optimizations. But you need more manual setup and management. Configuration of load balancers, VMSS, and other scaling components needs more effort and expertise.

- Availability:
  + Azure App service : App service has global scale with high availability. Using App service I can host my app anywhere in Microsoft's global datacenter infrastructure, and the App service SLA promises high availability.
  + Virtual machine : Vms has high availability options with Availability Sets and Zones and suitable for applications requiring specific configurations and high control over the environment

- Workflow:
  + Azure App service : Azure App service support automated deployments from Git Repository to Azure. It is very easy to upload my project changes to GitHub repository and then for the web app to take the project and deploy it to the web application.
  + Virtual machine : VMs requires manual installation and configuration of the operating system, application software, and dependencies. But you have fully control the OS, network, ....

- I chose the App service to implement for my project requirements based on the costs, scalability, availability, and workflow analysis. And that why i choose the App service:
  + My web applications need quick deployment, automatic scaling, and minimal management overhead. App service provides a simplified, managed environment with and managed by Azure, i don't want to care about the app's infrastructure, and set up environment manually
  + Azure app service allows me to quickly build, deploy and scale with auto-scaling and load balancing are integrated.
  + In this assignment, I used Azure Resource (Storage Account, Sql server and database) so i don't need to use VMs.
  + With my small web application, using App Service is more cost-effective. App service provides a managed environment with predictable pricing
### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
I must choose Virtual Machine instead of using App service in cases: 

- I want to control the underlying OS or install a software on the server. With App service I have limited access to the host server.

- App service has a hardware limitations. So if my app grows up, and the number of users increase or more features are added to the app, I would choose a Virtual Machine.


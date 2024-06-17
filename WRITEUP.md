# Write-up Template
something
### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
I chose the App service to implement for my project requirements based on the costs, scalability, availability, and workflow analysis. And that why i choose the App service:

- Cost: Azure App service is lower cost than a virtual machine. App service also has built-in load balancers that help save infrastructure costs.

- Scalability: I can easily increases or decreases resources allocated to my App service, such as the amount of vCPUs or RAM, by changing the App service pricing tier. With Auto scaling App service can automatically scale the number of instances based on a schedule or metrics like CPU, memory or HTTP queue length.

- Availability: Global scale with high availability. Using App service I can host my app anywhere in Microsoft's global datacenter infrastructure, and the App service SLA promises high availability.

- Workflow: Azure App service support automated deployments from Git Repository to Azure. It is very easy to upload my project changes to GitHub repository and then for the web app to take the project and deploy it to the web application.


### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
I must choose Virtual Machine instead of using App service in cases: 

- I want to control the underlying OS or install a software on the server. With App service I have limited access to the host server.

- App service has a hardware limitations. So if my app grows up, and the number of users increase or more features are added to the app, I would choose a Virtual Machine.


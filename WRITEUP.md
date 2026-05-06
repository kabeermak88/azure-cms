# Write-up Template

## Analyze, Choose, and Justify the Appropriate Resource Option for Deploying the App

This project involved deploying a Flask-based CMS web application using Microsoft Azure cloud services. Two deployment options were considered for hosting the application: Azure Virtual Machine (VM) and Azure App Service.

---

# Virtual Machine (VM)

A Virtual Machine provides complete control over the operating system and server environment. Developers can manually configure software, networking, dependencies, and security settings.

## Advantages of VM
- Full administrative control over the operating system
- Ability to install custom software and configurations
- Flexible environment for advanced applications
- Suitable for applications requiring specialized configurations

## Disadvantages of VM
- Requires manual maintenance and updates
- Higher management complexity
- Security patching and monitoring must be handled manually
- Longer deployment workflow

## Cost
Virtual Machines generally cost more because users pay for compute resources, storage, and uptime continuously.

## Scalability
Scaling a VM-based application requires manual setup such as load balancers, VM scale sets, or additional infrastructure configuration.

## Availability
Availability depends heavily on manual infrastructure configuration and maintenance practices.

## Workflow
Deployment using VMs involves configuring the operating system, installing dependencies, setting up the web server, and maintaining the infrastructure manually.

---

# Azure App Service

Azure App Service is a Platform as a Service (PaaS) solution that simplifies deployment and management of web applications.

## Advantages of Azure App Service
- Easy and fast deployment
- Managed infrastructure
- Integrated GitHub deployment support
- Built-in monitoring and logging
- Simplified scaling
- Reduced maintenance effort
- Suitable for Flask and Python applications

## Disadvantages of Azure App Service
- Less operating system control compared to VMs
- Limited customization options
- Some advanced configurations may not be supported

## Cost
Azure App Service provides affordable pricing plans including free and basic tiers, making it cost-effective for educational and small-scale projects.

## Scalability
App Service supports scaling through Azure Portal with minimal configuration effort.

## Availability
Azure handles infrastructure reliability, uptime management, and platform maintenance automatically.

## Workflow
The deployment workflow is simpler because App Service supports direct deployment from GitHub repositories and automatic build processes.

---

# Chosen Deployment Option

For this CMS application, Azure App Service was selected as the preferred deployment solution.

## Justification

Azure App Service was chosen because it simplifies deployment, reduces maintenance complexity, and integrates easily with GitHub. The CMS application does not require low-level operating system access or specialized infrastructure configurations.

The platform provides:
- Faster deployment
- Simplified application hosting
- Built-in scalability
- Integrated monitoring and deployment tools
- Lower maintenance overhead

Additionally, the free tier provided a cost-effective solution suitable for development and educational purposes.

---

# Assess App Changes That Would Change the Decision

The deployment choice could change depending on future application requirements.

A Virtual Machine would become a better choice if:
- The application required custom operating system configurations
- Specialized software or services needed installation
- Advanced networking or firewall configurations were necessary
- Multiple backend services required full infrastructure control
- High-performance computing or GPU workloads were needed

For large enterprise systems requiring extensive customization and infrastructure control, a VM-based deployment may provide greater flexibility.

However, for a standard Flask-based CMS web application, Azure App Service remains the most efficient, scalable, and manageable solution.
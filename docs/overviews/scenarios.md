# Scenarios 

This page is a starting point for understanding if some or all of the components are a fit for your edge use case.

It's intentionally informal so please feel free to [open a discussion](https://github.com/orgs/ubiquitous-factory/discussions) if more details are required. 

Q. I have 1 or 2 services that is unlikely to change in the near future what's the best option? 

   Consider using an image mode container such as [Mehal Coras](https://mehal.tech/coras) or [Fedora](https://docs.fedoraproject.org/en-US/bootc/getting-started/) with [Brog](https://github.com/mehal-tech/brog) and manage the deployment through OS upgrades and rollbacks.

Q. Due to Third Party compatibility issues I must use Ubuntu is there any benefit in using Ubiquitous Factory technology?

   Yes - If you are also deploying your own software onto the device you should consider using [Quadit](https://github.com/ubiquitous-factory/quadit)  so you aren't reliant on the providers operating system.

Q. I want the ability to distribute light weight workloads without pushing an operating system definition with the workload can Ubiquitous Factory help? 
   Yes - The [Amrite](https://github.com/mehal-tech/amrite) runtime can be dropped into your own operating systems definitions without any other Ubiquitous Factory components and workloads can be deployed as WASI binaries. 

Q. I'm currently using my own instance of [Open Horizon](https://open-horizon.github.io/) is there any additional value in adopting Ubiquitous Factory into my stack? 
   
   Yes - [Brog](https://github.com/mehal-tech/brog) can provide a way to manage your OS without interfering with your current application management system.

Q. My company has standardised on Circle CI for builds, uses bitbucket for source code and has there own private ECR instance on AWS. All of these services have enterprise controls in place can I still use Ubiquitous Factory?
   
   Of course - We have intentionally designed the system to integrate with industry standard devops tools - Ubiquitous Factory's aim is to utilse these services for the edge not rewrite them. See the [getting started](../howto/getting-started.md) for how external services are integrated. 

Q. The developers at my company prefer Docker over podman can we still use [coras](https://mehal.tech/login) to manage operating system updates? 

   Absolutely, and you can look at management systems such as Open Horizon to help you with the overall management.
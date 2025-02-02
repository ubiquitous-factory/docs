# Scenarios 

Now lets look at some scenarios: 

Q. I have 1 or 2 services that is unlikely to change in the near future what's the best option? 

   As the [Mehal Coras](https://github.com/mehal-tech/open-coras) is an image mode container you may want to consider just using [Brog]((https://github.com/mehal-tech/brog) to simply manage OS upgrades and rollbacks.

Q. Due to Third Party compatibility issues I must use Ubuntu is there any benefit in using Mehal Technologies?

   Yes - If you are also deploying your own software onto the device you should consider using [Quadit](https://github.com/ubiquitous-factory/quadit)  so you aren't reliant on the providers operating system.

Q. I want the ability to distribute light weight WASI workloads can  Mehal Technologies help? 
   Yes - The [Amrite](https://github.com/mehal-tech/amrite) runtime can be dropped into your own operating systems definitions without any other  Mehal Technologies components. 

Q. I'm currently using my own instance of [Open Horizon](https://open-horizon.github.io/) is there any additional value in adopting Mehal Technologies into my stack? 
   
   Yes - [Brog](https://github.com/mehal-tech/brog) can provide a way to manage your OS without interfering with your current application management system.

Q. My company has standardised on Circle CI for builds, uses bitbucket for source code and has there own private ECR instance on AWS. All of these services have enterprise controls in place can I still use Mehal Technologies?
   
   Of course - We have intentionally designed the system to integrate with industry standard devops tools - Mehal Technologies aim is to utilse these services for the edge not rewrite them. 

Q. The developers at my company prefer Docker over podman can we still use [coras](https://mehal.tech/login) to manage operating system updates? 

   Absolutely, and you can look at management systems such as Open Horizon to help you with the overall management.
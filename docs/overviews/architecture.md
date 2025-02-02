# Architecture 

The Ubiquitous Factory architecture is designed to be composable. Specifically the components are designed in such a way that they work together but each one can be deployed without a hard dependency on another. This is different than most vertically integrated IoT technologies that tend to be are tightly coupled and usually lead to the adoption of specific hardware and operating system and management systems. They also tend to be very prescriptive on how builds, deployment and overall management are performed.

The intent here is to embrace the cloud native ecosystem approach as much as possible to provide closer alignment with the way your whole business builds and deploys technology. 

Put simply: You shouldn't have to keep a gorilla just because you want a banana. 

The following diagram depicts how this point of view maps out in terms of the components in a typical smart edge deployment.

![component diagram](/assets/components.png)

[drawio version](/assets/components.drawio)
# Architecture 

The Ubiquitous Factory architecture is designed to be composable. Specifically, each components interface in such a way that they work together but a single one can be deployed without a hard dependency on another. A key priority for the project is that a fully functional system should be deployable with all the components without requiring any proprietary technology.

This is different than most vertically integrated IoT technologies that tend to hide the implementation details which can lead to a tight coupling scenario and this has the knock on effect of being difficult to integrate with other processes to the point where they also tend to be very prescriptive on how builds, deployment and overall management are performed.

The intent here is to embrace cloud native approaches as much as possible to provide closer alignment with the way a whole business builds and deploys technology not just to the edge but to the cloud. 

Put simply: You shouldn't get a gorilla just because you want a banana. 

The following diagram depicts how this point of view maps out in terms of the components in a typical smart edge deployment with comparable components from the eco-system to illustrate how different parts of the stack can co-exist together.

![component diagram](/assets/components.png)

[drawio version](/assets/components.drawio)
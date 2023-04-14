HI 

Azure Devops 
Kubernetes 
Terraform
Azure infra

Ans:
Microsoft-hosted agents
If your pipelines are in Azure Pipelines, then you've got a convenient option to run your jobs using a Microsoft-hosted agent. 
With Microsoft-hosted agents, maintenance and upgrades are taken care of for you.
Each time you run a pipeline, you get a fresh virtual machine for each job in the pipeline. 
The virtual machine is discarded after one job (which means any change that a job makes to the virtual machine file system, such as checking out code,will be unavailable to the next job).
Microsoft-hosted agents can run jobs directly on the VM or in a container.
Azure Pipelines provides a predefined agent pool named Azure Pipelines with Microsoft-hosted agents.

Self-hosted agents
An agent that you set up and manage on your own to run jobs is a self-hosted agent. 
You can use self-hosted agents in Azure Pipelines or Azure DevOps Server, formerly named Team Foundation Server (TFS). 
Self-hosted agents give you more control to install dependent software needed for your builds and deployments. 
Also, machine-level caches and configuration persist from run to run, which can boost speed.



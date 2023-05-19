
1.How to restrict access to the master branch in Git

To protect a branch:

On GitHub, navigate to the main page of the repository.

Under your repository name, click Settings.

In the left menu, click Branches.

Next to "Branch protection rules", click Add rule.

Under "Branch name pattern", type the branch name or pattern you want to protect (Impacted branches are listed and counted).

Configure specific branch rule settings if needed.

Click Create or Save changes.


1.https://stackoverflow.com/questions/38864405/how-to-restrict-access-to-the-master-branch-in-git


Azure Group ?

Groups are used to manage users that all need the same access and permissions for potentially restricted apps and servic

What is Kubernetes pod?
A Kubernetes pod is a collection of one or more Linux® containers, and is the smallest unit of a Kubernetes application. Any given pod can be composed of multiple, tightly coupled containers (an advanced use case) or just a single container (a more common use case). 
Containers are grouped into Kubernetes pods in order to increase the intelligence of resource sharing.

What is azure resource group?

A resource group is a container that holds related resources for an Azure solution.

![image](https://user-images.githubusercontent.com/30367367/232394645-d06f4774-9825-4a51-a95d-65f79dd981d2.png)


![image](https://user-images.githubusercontent.com/30367367/232394481-187e2d6a-e28c-4ce3-a999-1fe319023da5.png)




What is service prinicipal ?

Service Principal is an application within Azure Active Directory, which is authorized to access resources in Azure. This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level

Create a Service Principal.
Authorize and Assign a role to the Service Principal.
To associate a Service Principal with Serverless360, the following values are required:

Tenant Id - Azure Active Directory Id.
Client Id - Id of the Service Principal object / App registered with the Active Directory.
Client Secret - Application password.

https://docs.serverless360.com/docs/what-is-a-service-principal-1


05-05-2023:

https://azurecharts.com/

1.	Azure Active Directory
2.	Azure DNS
3.	Azure Firewall
4.	Azure Load Balancer
5.	Azure Bastion
6.	Azure Application Gateway
7.	Azure Kubernetes Services (AKS)
8.	Azure Monitor
9.	Azure Spring Cloud
10.	App Services
11.	Mobile Apps
12.	Logic Apps
13.	Azure Functions
14.	Azure Web Jobs
15.	Azure Event Grid
16.	Azure Service Bus
17.	Azure Storage (blob, tables, queues, file, disk)
18.	Azure CosmosDB
19.	Azure Cognitive Services
20.	Azure CDN (Content Delivery Network)
21.	Azure Redis Cache
22.	Azure API Management
23.	Azure SQL Managed Instance
24.	Azure Relational Databases (MySQL, PostgreSQL, SQL)
25.	Azure NoSQL Databases (MongoDB etc)
26.	Azure Data Lake Storage
27.	Azure Data Factory

8/5/2023:

What is helm?
Helm is a tool that automates the creation, packaging, configuration, and deployment of Kubernetes applications by combining your configuration files into a single reusable package.

What is helm chart?

A Helm chart is a set of YAML manifests and templates that describes Kubernetes resources (Deployments, Secrets, CRDs, etc.) and defined configurations needed for the Kubernetes application, and is also easy to deploy in a Kubernetes cluster or in a single node with just one command


9/5/2023:

K8s
helm deployment

12-05-2023:

1.Service principal in azure or management Identity 
2.Azure security 

15-05-2023:

What is difference b/w Rebase and Merge?

Merging is a safe option that preserves the entire history of your repository, 
while rebasing creates a linear history by moving your feature branch onto the tip of main

19-05-2023:

1.What is differebce b/w configmap and Secrets?
The big difference between Secrets and ConfigMaps are that Secrets are obfuscated with a Base64 encoding.
but it is good practice to use Secrets for confidential data (like API keys) 
and ConfigMaps for non-confidential data (like port numbers).

kubectl create secret generic apikey --from-literal=API_KEY=123–456

kubectl create configmap language --from-literal=LANGUAGE=English


2.What is difference b/w a replication controller and replica set?

The major difference between a replication controller and replica set is that the rolling-update command works with Replication Controllers,
but won't work with a Replica Set.  This is because Replica Sets are meant to be used as the backend for Deployments.

3. what difference b/w Deployments, statefulset and daemonsetes? 

Deployments are great for stateless applications that can be easily scaled horizontally.
StatefulSets are great for applications that require persistent storage and have state that needs to be maintained
DaemonSets are great for running an application on every node in the cluster.


4.What is auto scalling ?
Kubernetes enables autoscaling at the cluster/node level as well as at the pod level, two different but fundamentally connected layers of Kubernetes architecture.

5.How do you scale Kubernetes pods automatically?

Kubernetes Automatic Scaling with the Horizontal Pod Autoscaler (HPA) Object. 
The Kubernetes HorizontalPodAutoscaler object updates pods, deployments and statefulsets to match demands by automatically scaling workloads. 
The HPA's response to increased load is to dynamically provision additional pods











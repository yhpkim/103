# The very first step is to create a new namespace in each of our three clusters ps-dev, ps-prod, ps-prod2. We are going to use a spinnaker pipeline to do this. 

1.	Login to training.armory.io
2.	Configure an Application
 

2.	Click on Pipelines
3.	Click on Configure a new pipeline
4.	Name pipeline “deploy mcgonagle namespace in each cluster”
5.	Add a Deploy (Manifest) Stage
6.	Change Name to Deploy mcgonagle in namespace dev
7.	Account: eks-ps-dev
8.	Manifest Source → text
9.	Copy Deployment Manifest into TextBox
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/namespace.yml
10.	Click Save Changes at Bottom Right Screen
11.	Add a Deploy (Manifest) Stage
12.	Change Name to Deploy mcgonagle in namespace prod
13.	Account: eks-ps-prod
14.	Manifest Source → text
15.	Copy Deployment Manifest into TextBox
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/namespace.yml
16.	Click Save Changes at Bottom Right Screen
17.	Add a Deploy (Manifest) Stage
18.	Change Name to Deploy mcgonagle in namespace prod2
19.	Account: eks-ps-prod2
20.	Manifest Source → text
21.	Copy Deployment Manifest into TextBox
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/namespace.yml
22.	Click Save Changes at Bottom Right Screen
23.	Click Pipelines at top of screen 
24.	Run pipeline with a start manual execution

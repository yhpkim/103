# The very first step is to create a new namespace in each of our three clusters ps-dev, ps-prod, ps-prod2. 

# We are going to use a spinnaker pipeline to do this. 

1.	Login to training.armory.io
2.	Configure an Application
3.	Click on Pipelines
4.	Click on Configure a new pipeline
5.	Name pipeline “deploy mcgonagle namespace in each cluster”
6.	Add a Deploy (Manifest) Stage
7.	Change Name to Deploy mcgonagle in namespace dev
8.	Account: eks-ps-dev
9.	Manifest Source → text
10.	Copy Deployment Manifest into TextBox
`https://raw.githubusercontent.com/mcgonagle/103/master/manifests/namespace.yml`
11.	Click Save Changes at Bottom Right Screen
12.	Add a Deploy (Manifest) Stage
13.	Change Name to Deploy mcgonagle in namespace prod
14.	Account: eks-ps-prod
15.	Manifest Source → text
16.	Copy Deployment Manifest into TextBox
`https://raw.githubusercontent.com/mcgonagle/103/master/manifests/namespace.yml`
17.	Click Save Changes at Bottom Right Screen
18.	Add a Deploy (Manifest) Stage
19.	Change Name to Deploy mcgonagle in namespace prod2
20.	Account: eks-ps-prod2
21.	Manifest Source → text
22.	Copy Deployment Manifest into TextBox
`https://raw.githubusercontent.com/mcgonagle/103/master/manifests/namespace.yml`
23.	Click Save Changes at Bottom Right Screen
24.	Click Pipelines at top of screen 
25.	Run pipeline with a start manual execution

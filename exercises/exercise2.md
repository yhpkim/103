# Create a new Spinnaker Application
 

1.	Configure Application
 

2.	Click on Pipelines
3.	Click on Configure a new pipeline
4.	Name pipeline hundredthree
5.	Add a Deploy (Manifest) Stage
6.	Account: eks-ps-dev
7.	Manifest Source → text
8.	Copy Deployment Manifest into TextBox - https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
9.	Click Save Changes at Bottom Right Screen
10.	Click on Pipelines at top of screen
11.	Click Start Manual Execution
12.	Click Infrastructure at top 
13.	Click Load Balancers
14.	Click Plus Sign to add a load balancer
15.	Choose eks-ps-dev
16.	Copy LoadBalancer Service Manifest into text box- 
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/loadbalancer.yml

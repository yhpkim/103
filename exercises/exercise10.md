# Create a pipeline that deploys a stateful application, observe what happens when updated
1.	Click on pipelines
2.	Click on plus sign
3.	Click on add stage 
4.	Select type Deploy (Manifest)
5.	Stage Name Deploy Drupal
6.	Under Basic Settings → Account choose eks-ps-dev for the account
7.	Copy Deployment manifest into Manifest configuration
8.	https://raw.githubusercontent.com/mcgonagle/103/master/manifests/drupal_deployment.yml
9.	Click Save in bottom right hand corner
10.	Run Pipeline
11.	Click Save Changes at Bottom Right Screen
12.	Click on Pipelines at top of screen
13.	Click Start Manual Execution
14.	Click Infrastructure at top 
15.	Click Load Balancers
16.	Click Plus Sign to add a load balancer
17.	Choose eks-ps-dev
18.	Copy LoadBalancer Service Manifest into text box- 
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/drupal_loadbalancer.yml
19.	Connect to LoadBalancer address on port 8080
20.	Walk through Drupal Setup
21.	Choose English Language -> Save and Continue
22.	Choose Standard Installation -> Save and Continue
23.	Choose SQLite as the backend database leave default location -> Save and Continue
24.	Fill out configuration -> Save and Continue
25.	In the top left click content
26.	Click Add Content
27.	Click Basic Page
28.	Fill out Title and Body -> Click Save
29.	Page is Updated in Drupal
 
 
 
 

# Create a pipeline that promotes a manifest to production in two clusters concurrently
1.	Click on pipelines
2.	Click on plus sign
3.	Click on add stage 
4.	Select type Deploy (Manifest)
5.	Stage Name Deploy to Dev
6.	Under Basic Settings → Account choose eks-ps-dev for the account
7.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
8.	Click on add stage
9.	Stage name Deploy to Prod1
10.	Select type Deploy (Manifest)
11.	Under Basic Settings → Account eks-ps-prod
12.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
13.	Click back on Deploy to Dev Stage
14.	Stage name Deploy to Prod2
15.	Select type Deploy (Manifest)
16.	Under Basic Settings → Account eks-ps-prod2
17.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
18.	Click Save in bottom right hand corner
19.	Run Pipeline

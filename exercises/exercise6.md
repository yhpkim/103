# Create a pipeline that promotes a manifest from dev to production

1.	Click on pipelines
2.	Click on plus sign
3.	Click on add stage 
4.	Select type Deploy (Manifest)
5.	Stage Name Deploy to Dev
6.	Under Basic Settings → Account choose eks-ps-dev for the account
7.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
8.	Click on add stage
9.	Stage name Deploy to Prod
10.	Select type Deploy (Manifest)
11.	Under Basic Settings → Account eks-ps-prod
12.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
13.	Click Save in bottom right hand corner
14.	Run Pipeline

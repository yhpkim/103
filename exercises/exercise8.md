# Create a pipeline that promotes to two production clusters sequentially with a manual judgement
1.	Click on pipelines
2.	Click on plus sign
3.	Click on add stage 
4.	Select type Manual Judgment
5.	Under Instructions specify – Deploy to two clusters?
6.	Click on add stage
7.	Select type Deploy (Manifest)
8.	Stage Name: Deploy to Dev
9.	Under Basic Settings → Account choose eks-ps-dev for the account
10.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
11.	Click on add stage
12.	Stage name Deploy to Prod
13.	Select type Deploy (Manifest)
14.	Under Basic Settings → Account eks-ps-prod
15.	Copy Deployment manifest into Manifest configuration
https://raw.githubusercontent.com/mcgonagle/103/master/manifests/deployment.yml
16.	Click Save in bottom right hand corner
17.	Run Pipeline

# Create a pipeline that bakes and deploys the new manifest with a Docker trigger
1.	Go back into the pipeline you created in the first exercise
2.	Click Configure
3.	Click on the configure stage of the pipeline
4.	Under Automated Triggers click add trigger
5.	Under type select Docker Registry
6. Define Image Id -> Select from list
7. Registry Name -> dockerhub2
8. Organization -> mcgonagle
9. Image -> mcgonagle/103
10. Tag -> latest

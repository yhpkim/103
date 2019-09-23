# Create a Helm template
1.	Install helm
	1.	brew install kubernetes-helm
2.	helm create hundredthree
3.	cd hundredthree
4.	replace values.yaml with
`https://raw.githubusercontent.com/mcgonagle/103/master/helm/hundredthree/values.yaml`
5.	replace templates/deployment.yaml with
`https://raw.githubusercontent.com/mcgonagle/103/master/helm/hundredthree/templates/deployment.yaml`
6.	replace templates/service.yaml with
`https://raw.githubusercontent.com/mcgonagle/103/master/helm/hundredthree/templates/service.yaml`
7.	run ` helm install —name hundredthree ./hundredthree` 

8. run	`helm delete —purge hundredthree` to delete

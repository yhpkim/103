# Create a Docker image

1.	Install Docker Desktop
2.	`git clone git@github.com:mcgonagle/103.git`
3.	cd into 103
4.	`docker build --tag=mcgonagle/103 . && docker run -it --rm -p "9000:9000" mcgonagle/103`

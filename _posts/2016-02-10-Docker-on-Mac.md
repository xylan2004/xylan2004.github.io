## Install & Startup
In an OS X installation, the docker daemon is running inside a Linux VM called default. The default is a lightweight Linux VM made specifically to run the Docker daemon on Mac OS X. The VM runs completely from RAM, is a small ~24MB download, and boots in approximately 5s.

![docker on mac](https://docs.docker.com/v1.8/installation/images/mac_docker_host.svg)


## Mount Share folder
1. Set shared folder in VirtualBox

![VirtualBox](images/vituralbox-sharefolder.png)

2. Start docker container with -v option

<code>$ docker run -v /Users/bob/myapp/src:/src [...]</code>

Will mount the directory /Users/bob/myapp/src from your Mac into the container. This makes it much easier to use Docker for a continuous development flow, where you benefit from a predictable containerized development environment, but don’t want to rebuild a new container every time you change a line in your source code. If you are using Fig for your development workflow, for example, the benefits are immediately obvious.

Note that there are still some limitations: for example this feature is limited to boot2docker’s virtualbox configuration, cannot be managed dynamically, and only works for directories in /Users . But we are receiving exciting contributions to improve volume management, so expect this area to improve drastically in the next few releases.

# rocky-linux-9.6
Create a Docker container base image using Rocky Linux version 9.6 tar file

Step1: Load in your system, container tar file
Source: https://download.rockylinux.org/pub/rocky/9.6/images/x86_64/

```bash
wget https://download.rockylinux.org/pub/rocky/9.6/images/x86_64/Rocky-9-Container-Base-9.6-20250531.0.x86_64.tar.xz
```

Step2: extract  the xz  file

```bash
xz -d Rocky-9-Container-Base-9.6-20250531.0.x86_64.tar.xz
```

Step3: Create docker image

```bash
docker import Rocky-9-Container-Base-9.6-20250531.0.x86_64.tar rocky9:9.6
```

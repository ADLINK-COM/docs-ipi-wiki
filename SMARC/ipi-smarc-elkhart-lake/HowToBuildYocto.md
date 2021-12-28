# **How to Build Yocto**

<div class = "bullets">

The Yocto Project (YP) is an open source collaboration project that helps developers create custom Linux-based systems regardless of the hardware architecture. This procedure will help you build Yocto image for **I-Pi SMARC Elkhart Lake**

## **1. Set up a build host environment:**

### **Recommended Hardware for the host**

- Intel Core-i7 Processor (>= 4 cores)
- at least 8GB Memory
- at least 500GB Disk space
- Ubuntu **18.04 LTS 64bit** or later version for Yocto Project Build
- High speed network connectivity 

<br>

### &nbsp;**Essential host Packages required to be installed in your host :**

```python
$ sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib \
 build-essential chrpath socat cpio python python3 python3-pip python3-pexpect \
 xz-utils debianutils iputils-ping python3-git python3-jinja2 libegl1-mesa libsdl1.2-dev \
 pylint3 xterm
```

**Note:**

Please **Don't** use the root account to build Yocto. It might cause unpredictable errors. 

<br>

### **"Google repo" packages required to be installed in your host :**

```shell
$ mkdir ~/bin (this step may not be needed if the bin folder already exists)
$ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$ chmod a+x ~/bin/repo
$ export PATH=${PATH}:~/bin
```

<br>

### **Before starting to build the source, make sure that git is set up properly with the commands below:**

```shell
$ git config --global user.name "Your Name"
$ git config --global user.email "Your Email"
$ git config --list
```

<br>

## 2. Fetch the source from the git location as below:

**Create the working directory as we have to create "imx-yocto-bsp"**

```shell
$ mkdir imx-yocto-bsp 
$ cd imx-yocto-bsp
```



**Start to download the source ** 

```shell
$ repo init -u https://github.com/ADLINK/adlink-manifest -b lec-imx-yocto-zeus -m adlink-lec-Elkhart-Lake-yocto-zeus_1v1.xml
$ repo sync
$ MACHINE=lec-Elkhart-Lake DISTRO=fslc-xwayland BUILD=build source adlink-imx-setup-release.sh
```

### 3. Build the Image

Choose the Image recipe with the supported hardware

| Module name                              | Yocto branch | bitbake command                  |
| :--------------------------------------- | :----------- | :------------------------------- |
| lec-Elkhart-Lake + Wayland desktop (GUI) | zeus         | `$ bitbake imx-image-multimedia` |
| lec-Elkhart-Lake + console (CLI)         | zeus         | `$ bitbake core-image-minimal`   |

After the build is complete, disk images will be located at work-dir/build-dir/tmp/deploy/image/lec-Elkhart-Lake/ 

### Image is generated as wic.bz2, use below command to unzip

```shell
$ bunzip2 -dk -f <image_name>.wic.bz2
```

</div>

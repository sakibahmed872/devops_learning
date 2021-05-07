# Class Two

What I am learning from second class. 

___

## Virtual Machine
We used Virtual machine to utilized our resourses. We can divide resourses by Virtualizing the resourses. Virtual Machine can divide OS, CPU, RAM, Storage etc. 

In a Computer, by installing a hypervisor we can make the virtualization. Hypervisor works above the OS of a computer.


Virtual Machine also need an OS and all necessary dependencies. In a physical Computer, if we run multiple virtual machines, all the machines requires to Install OS and all necessary dependencies.


## What is Docker? 

Docker is a packaging system that keeps the application identical. Docker use OS level virtualization and deliver a package called container. Docker use Linux Kernel features like namespaces. Docker-Container can only be used in Linux. We can run as many as containers as we want. We can scaling the number of containers anytime. This is called Horizontal scaling. We don't need to install OS for each container. 


> We use Virtual Machine and Container together. We actually run the container inside a virtual machine. 


## Markel Tree
Markel Tree or hash Tree is used for data verfification and synchronization. It is used to verify stored data and transferred data. If there is any changes while transfering, Hash key of both file won't be same. This key is ensure that both the files are same and there was no error while transfering to other computer.

For a large file, while tranfering system breaks the file in many chunk(part) and send the file with hash key. after tranfering, hash key is checked. If not same, re-send that file again not the entire big file. This is a great usage of markel tree or hash tree.


## How to install Docker or Docker Host

1. Installation in Manjaro OS
   Open your terminal and run the following command to download and install docker. Internet Connection is required.

   ```bash
   $ sudo pacman -S docker
   ```

   This will automatically download and install latest verison of docker.

   The next step is to start the docker service. follow the commad. You can optionally run the next line to run the docker when booted.

   ```bash
   $ sudo systemctl start docker.service
   $ sudo systemctl enable docker.service
   ```
   Now its time check verify the installation and check the version.
   ```bash
   $ sudo docker version
   ```
   You will see the version and details of Docker. You have successfully installed Docker in your machine.

   

# Reference
* [Markel Tree](https://en.wikipedia.org/wiki/Merkle_tree)


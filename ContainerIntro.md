# Before we dive into Kubernetes, we must understand what a Container is!

## Container 

#### Need for Container?

###### Traditional architecture

All the softwares are developed for a particular OS version and 
While installing the software we go through the below procedure as there would be a lot of dependencies issues.


###### Software developers’ issues

- They had to build their softwares differently for each operating system in the market.
- **Each developer could use a different version which causes issues.**
    - Dev 1 uses python2
    - Dev 2 uses python3
    - This might cause issues.
- Each Team could use a different OS version.
    - Dev ubuntu 18.1
    - Testing ubuntu 20.1
    - Production server ubuntu 21.1
    - This might again cause issues.

###### Compatibility issues of the application.

- app1 requires python2 and ubuntu 19
- app2 requires python3 and ubuntu 20
- app3 requires python2.9 and ubuntu 22

We configured app1 now and it's running properly.

We are configuring app2 and fixing the dependency issues.

Now App1 doesn’t run properly and we have to a totally different configuration for app3

- This compatibility issue in the matrix of applications are usually referred to as "Matrix of Hell"
- Every time a developer makes some changes we have to go through the same process of fixing the dependency issues.
- Our application runs on Linux, But what if developers don't want to leave Windows as they are comfortable with it?

To fix the above issues, Container technologies were introduced!


- With containers we can isolate all the applications with their dependencies as if like a virtual server.
- Everyone including the dev/test team can run these containers easily in their computer to develop the applications.

### Benefits of containers.

- Easy to build and ship
- Build once and use everywhere
- Can have even different linux OS for different Applications running in the same machine.
- Only have to Install Docker(Container technology) and run their applications easily.


# Docker

Docker is a technology designed to make it easier to create, deploy, and run applications by using containers.

- Containerization tool
- As we see in the Logo, it's used to build and ship containers :)
- Open Source
- It follows the build once, run anywhere approach.


## What is Docker ?

**Docker is a Containerization Platform which allows us to containerize an application/software (called as Docker Image) & also lets you run Containerized application/software**

Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers.


Docker Shares the Kernel

- Docker does not contain the kernel
- It contains only the lib files and other things.
- Cannot run windows as a container.

##### DockerHub

Most companies have their software hosted as images in DockerHub.

##### Container Vs Images.

- Image - it's a package or template.
- Container = Running instance of an image.
- If you can't find the image in dockerhub, create one and upload it.

### Deployment Models (VM vs Containers)

![VMvsContainter](https://user-images.githubusercontent.com/91851332/145317900-15747f1f-e22f-4651-9caa-4648d31cffc6.png)

# Docker Advantages

- Resource savings (no additional OS files or OS processing needed)
- Does Not take any time to power on
- very fast
- Collaboration (sharing with others)
- cost - effective (run a lot of containers in a single server)
- Use it anywhere
- Developers create the dockerfile
- OPS team just use the image and deploy it in Production.







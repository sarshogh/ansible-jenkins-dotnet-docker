# Ansible playbook to install Jenkins Server from a Dockerfile (Customized with .Net5) 

 A simple Ansible playbook to build and run Jenkins Master Node from a dockerfile 
 
It is a customised Dockerfile to install Jenkins, .Net5 and Blueocean all together your local machine/server; and at the end runs a instance/container of that image with previligaed=true flag

To access to container and check all installation have been done properly you can run:

```
docker exec -it jenkins-master sh

> which dotnet
```


## Network access for your Jenkins Container
Since your jenkins gets run inside a docker container, you need to customise the 'docker run' command your network and volume which can simply gets added to main.yml playbook


## Content:
A Dockerfile which has a Jenkins installations along with BlueOceanUI and .Net5 SDK

### Prerequisites
 - install python3
 - install pip
 - install docker using pip
 - install ansbile using pip
  

## how to run locally
```
ansible-playbook main.yml
```

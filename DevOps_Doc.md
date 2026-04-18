       https://github.com/imnowdevops/ddc-material/archive/refs/heads/master.zip



       https://github.com/imnowdevops/ddc-material.git

 



Vagrant

---



Open git bash and enter commands to run vagrant Linux machine



cd /c

cd /vagrant files

cd /unix or /centos

vagrant up



vagrant global-status   // to check which vm is running



vagrant ssh   //To login



free -m // checking ram consumption





-----PACKAGE MANAGEMENT-------

yum and dnf  for redhat Linux (centos etc)



dnf is new command. It is more usefull.







----------------------------**GIT HUB---------------------------**



**-> Git is a version control system.**



**Version control system is a managing multiple version of**



\*\*\\\*Documents\*\*

	\*\*\\\*Programs\*\*

	\*\*\\\*Websites,  etc..\*\*






**Tracks history of collection of files**



**Version Control** Software keeps track of every modification to the code in a special kind of database





***Localized and centralized VCS***



* A localized version control system keeps local copies of the files.
* In centralized source control, there is a server and a client. The server is the master repository which contains all of the versions of the code.



---------------VERSIONING--------------------



//git add . command is used to track all the files.



//git status command is used to check if the files are tracked or not.



If we change the file in local. Command should be follow.

git add <file name>   // We do staging or index them.

git commit -m "saturns moons."  //To commit  'saturns moons' is a meaasage.

git push origin main //This is push changes in repository.

git pull // To Pull the changes to local.



-----git in command line----

git log //to login in command

git log --oneline //to commit id or details in small



--------BRANCHES-----------

git branch -c <branch name> //To create branch

git branch -a //To list the branches

git checkout/switch <branch name> // To switch to branches

git rm //To remove the files

git mv //To rename the file.

git push origin <branch name> //To push the branch.

git merge <branch name> //To merge changes of other branches to main. "Note:- You should be in branch which want to change."

git push --all origin //To push all the branches.

rm -rf <repo name> //To remove the repo.



-------------ROLLBACK--------------

git checkout //if want to undo the file before stagging

git diff //if want to check the difference of file before stagging

git diff --cached //if want to check the difference of file after stagging

git restored --staged <file name> //if want to Undo the file after stagging

git revert HEAD //if want to undo the file after commiting



-----------GIT TAGS--------------

TAG A COMMIT

git tag <TagName> commit
git show tag



ANNOTATED TAGS

git tag -a <TagName -m "message" \[commit]
git tag -a v2.1.6 -m "Release for something."



PUSH TAGS
git push origin tag TagName
git push --tags



------------------------VAGRANT----------------------------

Vagrant global-status  //shows the all the available vagrant VM's

Vagrant destroy --force //To del vagrant VM's

Vagrant global-status --prune //It shows the status of vm's with updated

Vagrant destroy <Id of the Vm's> //we can deletes the vm without entering to folder.

Vagrant halt //to off vagrant

Vagrant reload //To reboot the vagrant

vagrant box list //to list the vagrant file

vagrant init <box name> //to start the vagrant file

vagrant up //to power on vagrant

vagrant ssh //to login to vagrant machine

sudo -i //to become root



-----------How to build systemctl if it not works for some service like  apache tomacat-------------(If there is no default systemctl)--------

/usr/sbin/httpd $OPTIONS -DFOREGROUND //
When we run systemctl start service  it runs this command in background

----------JASON and YAML through Python Data Structure-----------------

----Lists----
tools=\["Jenkins","Docker", "KBs", "Terraform", 80"] //If it separated by commas in python and json then it is lists
print(tools) //It prints \["Jenkins","Docker", "KBs", "Terraform", 80"]
print(tools\[1]) //It prints Docker

print(tools\[1:4]) //it prints \['Docker', 'KBs', 'Terraform']

print(tools\[1:4]\[1]) //it prints KBs

----Tuple----
tools=("Jenkins","Docker", "KBs", "Terraform", 80") //lists in square bracket and tuple is in paranthesis.

print(tools) //It prints ("Jenkins","Docker", "KBs", "Terraform", 80")

----Dictionary-------

In dictionary  there will be key and value. it in curly braces.

devops={"skills":"devops","year":2025,"Tech":"","GitOps":""}
print(devops)

//In dictionary we dont have index number we have key name.

print(devops\["year"]) //This will print 2025



--------JASON AND YAML---------

devops={
"Skill":"DevOps",
"Year":2025,
"Tech":{
"cloud":"AWS",                ----------------->PYTHON
"CICD":"Jenkins",
"Containers":"KBs",

&nbsp;   "GitOps":\[
        "Gitlab",
        "ArgoCD",
        "Tekton"
        ]






{
"Skill":"DevOps",
"Year":2025,
"Tech":{
"cloud":"AWS",
"CICD":"Jenkins",
"Containers":"KBs",       ---------------->Json

&nbsp;   "GitOps":\[
        "Gitlab",
        "ArgoCD",
        "Tekton"
        ]
	}

}



devops:
Skill: DevOps
Year: 2025
Tech:                           ---------------------->YAML
Cloud: AWS
CICD: Jenkins
Containers: KBs
GitOps:
- Gitlab
- ArgoCD
- Tekton





---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------VPROFILE PROJECT SETUP \[LOCAL] ----------------------------------------------------------------------



It is a website written in JAVA consisting of multiple services we will be deploying this product on 5 VM's. Here we having 5 services running on different VM's. We will working on production while we keeping it on local for experiment.



----In this project we are going to set-up web application stack----



---SCENARIO:
Lets say we are working in a project.

In our project we have variety of services that powers up our project run time like DB sarvices(MySQL, PostgreSQL) Web services(Apache, ngnix).



------OBJECTIVE-------
VM AUTOMATION LOCALLY.

BASELINE FOR UPCOMING PROJECTS.

REAL WORLD PROJECT SETUP LOCALLY \[FOR R AND D].



ARCHITECTURE OF PROJECT SERVICES.

* NGNIX
* TOMCAT
* RABBITMQ
* MEMCACHED
* MYSQL

ARCHITECTURE OF AUTOMATED SETUP

* VAGRANT
* VIRTUAL box
* GITBASH

SATCK -----> Collection of services working together to create an experience.

* NGNIX -> Nginx (pronounced engine-x) is a web server — software that delivers websites or web applications to users over the internet.
* APACHE TOMCAT -> Apache Tomcat is an application server (or servlet container) used to run Java-based web applications.
* RABITMW -> RabbitMQ is a message broker — a system that helps applications talk to each other asynchronously by sending and receiving messages through a queue.
* MEMCACHED ->Memcached is an in-memory caching system used to speed up websites and applications.
  It temporarily stores data (like database query results or API responses) in RAM — so the app can get data much faster instead of going to the database every time.



---------------------------------------------------------------------------------------------------NETWORKING---------------------------------

CONTENTS

1. Components
2. OSI Model
3. Classification
4. Devices
5. Home Network
6. IP Addresses
7. Protocols
8. DNS \& DHCP
9. Network Commands.



International standard organization (ISO) has developed Open system Interconnection (OSI)

OSI is model of communication is used in computer network.

The basic elements of a layered model are.
\* Services
\* Protocols
\* Interfaces

1. A service is a set of actions that a layer offers to another (higher) layer
2. A protocol is a set of rules that a layer uses to exchange information.
3. A interface is communication between the layers.



Switches --> Switches facilitate the sharing of resources by connecting together all the  devices, including computers, printers  and servers in a small business network.

Routers --> A router receives and sends data on computer networks. Routers are sometimes confused with network hubs, modems, or network switches. However, routers can combine multiple networks together.



Private IP ranges

Class A -> 10.0.0.0 - 10.255.255.255

Class B -> 172.16.0.0 - 172.31.255.255.255

Class C -> 192.168.0.0 - 192.168.255.255



tracert -> trace-route command is used to trace the flow of packets from src to destination.

netstat antp -> this command is used to check which port is used by service.

ss -tunlp -> same command as netstat

nmap -> show the which port is open on server and which service is running.

dig -> DNS lookup

nslookup -> an older version of dig command

route -> this command will show gateway.

arp -> shows the record of map address.

mtr -> This command is traceroute but it shows in live.

telnet -> this command to connect with the port.



-----------------------------------------------------------------------------------------------------CONTAINERS-------------------------------

A software container is a lightweight, standalone, executable package of software that bundles an application's code with all its dependencies, such as libraries, binaries, and configuration files

DOCKER.

Docker is an open platform for developing, shipping, and running applications(Containers). Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications.



docker run <image-name> //this command runs container and if it is not available in locally. It will go and download the image in registry

docker images //this command is to list the docker images locally.

docker ps //this command shows the running containers

docker ps -a //this command shows all conatiners

docker inspect <container name> //this shows the ip address of the containers

docker stop <container name> //to stop the containers

docker rm <container name> //to remove the container

docker rmi <container name> //to remove the images

docker compose //to run multiple commands

docker compose need to compose file to run the containers

docker compose up //to run the multiple containers

docker compose ps //to check the running container.

docker compose down //this go and stops the container and remove it

docker system prune -a //this remove all the container and image as well.

---

// This is to tackle certificate error while runnine docker compose up//

Step 3 — Allow insecure registries (temporary fix)

Create or edit:

sudo nano /etc/docker/daemon.json



Add this content:

{
"insecure-registries": \["registry-1.docker.io"]
}



If you’re using a private registry, replace registry-1.docker.io with your registry domain.

Then restart Docker:

sudo systemctl daemon-reexec
sudo systemctl daemon-reload
sudo systemctl restart docker



Try again:

## docker compose up -d



\_\_\_***BASH SCRIPTING***

\#!/bin/bash

\#########This Script prints system info ###########

echo "Welcome to bash scripts."
echo

\#Checking system uptime
echo "#########################"
echo "The uptime of the system is:"
uptime
echo

\#Memory utilization
echo "######################"
echo "Memory utilization"
free -m
echo

\#Disk Utiliztion
echo "#######################"
echo "Disk Utilization"
df -h



\########Script to setup Website###########

#### Creating Temp Directory

mkdir -p /tmp/webfiles

cd /tmp/webfiles

echo "Starting Deployment"
echo "###########################"

sudo wget --no-check-certificate https://www.tooplate.com/zip-templates/2140\_stellaris\_research.zip

unzip 2140\_stellaris\_research.zip > /dev/null

sudo cp -r 2140\_stellaris\_research/\* /var/www/html

sudo systemctl restart httpd

rm -rf /tmp/webfiles

ip addr show | grep 192.168

sudo systemctl status httpd

\#######################################################################

\############COMMAND LINE ARGUMENTS################

Command line arguments in a Bash script provide a mechanism to pass data to the script at the time of its execution, allowing for dynamic behavior and user interaction.

\#!/bin/bash

#### This script setup website

# Variable Declaration

packages="httpd wget unzip"
svc="httpd"
tempdir="/tmp/webfiles"

# Installing Dependencies

echo "Installing Packages"
echo "#############################"
sudo yum install $packages -y > /dev/null

# Start and Enable Service

echo "##################################"
echo "Start and enable HTTPD Services"
echo "##############################"

sudo systemctl start $svc
sudo systemctl enable $svc

#### Creating Temp Directory

mkdir -p $tempdir

cd $tempdir

echo "Starting Deployment"
echo "###########################"

\#here $1 is used as command line argumenent (to take input from user)
sudo wget --no-check-certificate $1 > /dev/null

unzip $2.zip > /dev/null

sudo cp -r $2/\* /var/www/html

sudo systemctl restart $svc

rm -rf /tmp/webfiles

ip addr show | grep 192.168

sudo systemctl status $svc



\#######################COMMAND SUBSTITUTION####################

Command substitution is method of storing OUTPUT of a command into variable.

VarName = `Command`
VarName=$(Command)

\##########EXPORTING VARIABLES###############

Exporting variable will make the variable global for all the child shell

To export variables permanently. you can add the export command in any of the following start-up files:

* ~/.profile
* ~/.bashrc
* /etc/profile

Season="monsoon"
export season //by running this it will global. But this is still temporary if we logout it will vanish

To make permanent we need to add in .bashrc file. this will become permanent for root user.
If we need to make permanent for any other user then we need to add in their .bashrc file

If we need to make permanent for global user then we to add in /etc/profile

\#####################USER INPUT#############################

Taking input from the user while executing the script, storing it into variable and then using that variable in our script.

read var1

read is the command and var1 is variable. It takes the user input and stores it in var1



\#!/bin/bash

echo "Enter your skills"

\#here read is the command and skills is the variable that stores the user input.read SKILLS

echo "your $Skills skill is in high Demand in the IT Industry."

# here -p is for prompt to show username on screen

read -p 'Username: ' USR

# here -sp, s is for supress the what we type and p is prompt to show password

read -sp 'Password: ' pass

echo

echo "Login Successfull : Welcome USER $USR. "



\###############DECISION MAKING#####################
If statements



if \[<some teat> ]
then
<command>
fi

\#!/bin/bash

value=$(ip addr show | grep -v LOOPBACK | grep -ic mtu)

if \[ $value -eq 1 ]
then
echo "1 Active Network Interface found"
elif \[ $value -gt 1 ]
then
echo "Multiple active Interface."
else
echo "No active Interface found"
fi



\****SYSTEM MONITERING***

\#!/bin/bash

echo "\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*"

date

ls /var/run/httpd/httpd.pid \&> /dev/null

if \[ $? -eq 0 ]
then
echo "Httpd process is running"
else
echo "Httpd process is not running"
echo ""
echo "Starting the process"

systemctl start httpd
if \[ $? -eq 0 ]
then
echo "Process started succeccfully"

else
echo "Process strting failed, contact the admin"

fi
fi
echo "\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*"



\########################## LOOPS ################################

for var in <list>

## do

---

done

---

\#!/bin/bash

for var1 in java c python ruby php
do
echo "Looping..."
sleep 2
echo "######################"
echo "value of var1 is $var1."
echo "######################"
date
done

---

\#!/bin/bash

Myusers="alpha beta gama sigma"

for usr in $Myusers
do
sleep 1
echo "Adding User $usr"
useradd $usr
id $usr
echo "#######################"
done

---

\##################### WHILE LOOP ##############################

\#!/bin/bash

counter=0

while \[ $counter -lt 5 ]
do
echo "LOOPING"
echo "Value of counter is $counter."
counter=$(( $counter + 1 ))
sleep 2
done

echo ""
echo "out of the loop"



-------------------------CLOUD COMPUTING-------------------------------

https://aws.amazon.com/about-aws/global-infrastructure/regions\_az/



EC-2 -> EC2 is an elastic cloud computing.

1. On Demand -> Pay per hour or Seconds.
2. Reserved -> Reserve Capacity(1 or 3 yrs) for discounts.
3. Spot -> Bid your price for unused ec2 capacity. (we get huge discounts)
4. Dedicated Hosts -> Physical server dedicated for you. (Very expensive)



AMI -> Amazon machine image(AMI) provides the info required to launch an instance, which is a virtual server in the cloud.

Instance type -> type of instances.

EBS -> Amazon elastic block store, Amazon ec2 provides you with flexible, cost effective, and easy to use data storage options for your instances. ( Virtual hard disk) to store data

Tags -> to set names to filter.

Security Groups -> A security group acts as a virtual firewall that controls the traffic for one or more instances.

Key-pair -> Amazon EC2 uses public-key cryptography to encrypt and decrypt the login information. (to SSH)

Key-pair -> It is region specific. Different environment should have different key.

Eg:- If i created for north virginia. we can only use this key for north Virginia

**EC2 instance creation**

1. Requirement Gathering.
2. Key pairs
3. Security group
4. Instance launch

----Requirement Gathering----

1. OS
2. Size -> Ram, CPU, Network etc
3. Storage size
4. Project
5. Services/Apps Running (SSH, Http, MySQL, etc..)
6. Environment (Dev, QA, Staging, Prod)
7. Login User/ Owner

----KEY PAIR----

Key-pair -> It is region specific. Different environment should have different key.

Eg:- If i created for north virginia. we can only use this key for north Virginia

----SECURITY GROUPS----

* A security group acts as a virtual firewall that controls the traffic for one or more instances.
* You can add rules to each security group that allow traffic to or from its associated instances.
* Security groups are "Stateful".

Inbound :-  Traffic coming from outside on the instance

Outbound:- Traffic going instance to outside.



-------------------AMAZON CLI-----------------------------------

Authenticate in awscli for aws login

aws configure // this command is  this will ask access key, which we have created user in aws console.

$ ls ~/.aws/  // this is to check the config and credentials.

aws sts get-caller-identity // this command is to check if user is configurd.

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-prereqs.html   // Link to awscli documnets

------------------AWS SYSTEMS MANAGER ANS CLOUD SHELL-----------------

Aws system manger is used to handle many nodes(servers) at a time.

* AWS SYSTEM MANAGER can get direct ssh session to our instances with need of any authentication
* If we need to execute one command on 100 servers then we can use AWS SYSTEM MANAGER  (Like restarting a service or installing a service on 100 of server)
* To connect ec2 instances SSM we need some permissions. This permissions are given through IAM(ROLES).

(IAM)Roles -> It is used to connect one AWS service to another service. (Like ec2 wants to connect SSM)



---------------------------EBS (ELASTIC BLOCK STORAGE)-----------------

This is a virtual hard disk for our ec2 instances.

* Block based storage.
* Runs ec2 OS, store data from db, file data, etc
* Placed in specific AZ. Automatically replicated within the AZ to protect from failure.
* Snapshot is backup of a volume.
* EBS and ec2 should be in same AZ.

*EBS Types.*

1. General Purpose (SSD)

   * Most Work Loads

2. Provisioned IOPS

   * Large Databases

3. Throughput optimized HD

   * Big Data and Data Warehouses

4. Cold HDD

   * File Servers

5. Magnetic

   * Backups and Archives



--------------SNAPSHOTS------------------

* SNAPSHOTS are the backup of the EBS volumes.



------------------AWS CLOUD WATCH--------------------

* Cloud Watch- Monitor performance of AWS environment- standard infrastructure metrics.
* Metrics
  AWS cloud watch allows. you to record metrics for services such as EBS, EC2, ELB, Route53 Health checks, RDS, Amazon S3, cloudfront etc...
* Events:
  AWS Events delivers a near real-time stream of system events that describe changes in Amazon Web Services(AWS) resources.
* Logs:
  You can use amazon CloudWatch Logs to monitor, store, and access your log files from Amazon Elastic Compute Cloud (Amazon EC2) instances, AWS CloudTrail, Route 53, and sources.



* ALARM :- Alarm monitors cloudWatch metrics for instances.
* SNS(Email Notification) :- Simple Notification Services (Amazon SNS) is a web service that coordinates and manages the delivery or sending of messages to subscribing endpoints or clients.

  * If CPU utilization crosses 60%, then I should  receive email.

EC2 Instances ------> Amazon CloudWatch ------> Alarm -----> Email(SNS)
Create Alrm                             alrm triggered





--------------------AWS ELS (Elastic File System)----------------------

Amazon EFS is the shared file system.

Amazon Elastic File System (Amazon EFS) provides a simple, scalable, fully managed elastic NFS file system for use with AWS Cloud services and on-premises resources. It is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files, eliminating the need to provision and manage capacity to accommodate growth. Amazon EFS is designed to provide massively parallel shared access to thousands of Amazon EC2 instances, enabling your applications to achieve high levels of aggregate throughput and IOPS with consistent low latencies.



* Shared File System

The shared file system has centralized storage to all the servers.

Every server as there own block storage to store OS. BUT,
Like images, videos, Documents are shared in centralized storage

-> In Linux most shared protocol is NFS

-> To build NFS shared storage we need to host NFS server which contains all the hard disk.



---------------------------------AUTO SCALING-----------------------------------

Auto Scaling is a service that automatically monitors and adjusts compute resources to maintain performance for applications hosted in the AWS.

* If CPU utilization crosses threshold then it adds more video.
* Alarm monitors cloudwatch metrics for instances.



A launch configuration/Template is an instance configuration template that an auto scaling group uses to launch EC2 instances.



Scaling policy is used to increase and decrease the number of running instances
in the group dynamically to meet changing conditions.



------------------------------S3 (Simple Storage Service)-----------------------

Amazon Simple Storage Service (Amazon S3) is storage for the internet. You can use Amazon S3 to store and retrieve any amount of data at any time, from anywhere on the web.

S3 Basics

* It is Object-Based storage
* Data is replicated across multiple facilities
* Unlimited Storage
* Amazon S3 stores data as objects within buckets

\*\* Bucket name has to be unique \*\*



A bucket is a logical unit of storage in Amazon Web Services (AWS)

Object Storage is a computer data storage architecture that manages data as Objects.



Amazon S3 --> Bucket --> Folder --> object --> Public Access

S3 Storage Classes.

1 S3 Standard:
2 S3 IA- Infrequent Access
3 S3 One Zone-IA
4 S3 Intelligent Tiering
5 S3 Glacier
6 S3 Glacier Deep Archives


S3 Charges.

* Storage 
* Requests  (I/O)
* Tiers
* Data Transfer
* Region Replication


-----------------------------------RDS---------------------------------

RDS -> Relational database

* Amazon Relational Database Service is a distributed relational database service.

* High Availability Multi-AZ Deployments.

* Effortless Scaling.

* Read Replicas for performance.

 mysql -h vprofilemysqlserver.cnamkky685d2.us-east-1.rds.amazonaws.com -u admin -p

here, 
	-h is hosts and -u is user and -p is password





-------------AWS Cloud for project(V-profile) set up | Lift & Shift ---------

We are going to run (V-Profile) project on AWS cloud platform to Production.

*********ARCHITECTURE OF AWS SERVICES FOR THE PROJECT******* 

> EC2 Insatnces
> ELB
> AUTOSCALING
> EFS/S3 FOR SHARED STORAGE
> AMAZON CERTIFICATE MANAGE
> ROUTE 53

****FLOW OF EXECUTION****

1. Login to AWS Account 
2. Create Key Pairs
3. Create Security groups
4. Launch Instances with user data [BASH SCRIPT]
5. Update IP to name mapping in route 53 
6. Build Application from source code (In Local Machine)
7. Upload to S3 bucket
8. Download artifact to tomcat EC2 Instances.
9. Setup ELB with HTTPS ( Cert from Amazon Certificate Manager )
10. Map ELB Endpoint to website name in  Godaddy DNS
11. Verify
12. Build Autoscaling Group for Tomcat Instances.


If we want to push artifact to S3 bucket we need...

*Build artifact with Maven (It is build tool. We use to build artifact and maven needs JDK. Build artifact from source code)
* AWS CLI to push (To push artifact to S3 and communicate with that)
* Artifact to S3 (Uploading artifact to S3 bucket)


mvn install // this command is use to bulid artifact.


$ aws s3 cp target/vprofile-v2.war [Source] s3://vprofile-artifacts2001/ [Dstination]   //This command is used to copy the file from my computer to  aws s3 bucket.


aws s3 ls  s3://vprofile-artifacts/  //To list the files in s3 bucket.


aws s3 ls s3://vprofile-artifacts2001/
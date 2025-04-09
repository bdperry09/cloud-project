<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Set Up a Web App in the Cloud

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-devops-vscode)

**Author:** Brandon Perry  
**Email:** bdperry09@gmail.com

---

## Set Up a Web App Using AWS and VS Code

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_7a1de541)

---

## Introducing Today's Project!

In this project i am going to launch an EC2 instance, use VS code to connect to that instance using SSH and form there generate a basic web application with the help of Maven and JAVA.

### Key tools and concepts

Services I used were EC2, Iam, Vs code, linux, java and Maven

### Project reflection

I did'nt expect to have to troubleshoot VS code not connecting to my EC2 instance. Using a t2.micro type, the cpu would max out when trying to edit my web app. causing me to have to start and stop the instance to reconnect. 

This project took me approximately an hourto complete.The most challenging part was the instance cpu maxing out and VS Code dissconnecting.  It was most rewarding to fully comlete the project and understand exactly what i was doing along the way. 

This project is part one of a series of DevOps projects where I'm building a CI/CD pipeline! I'll be working on the next project in the upcoming days 

---

## Launching an EC2 instance

I started this project by launching an EC2 instance because of the customization an AWS EC2 instance provides. 

### I also enabled SSH

I enabled SSH so that I am able to securly connect to my EC2 instance from my home computer.

### Key pairs

A keypair is like your housekey and your frontdoor. Meaning they are unless without each other. If you lose your key, you are still safe because no one knows where you live. Your private key is safe as long as no one can associate it with the public

Once i set up my key pair, AWS automatically downloaded the github private key.

---

## Set up VS Code

VS code is an open source code editor 

I installed VS code to communicate with my EC2 instance and get more fimiliar with the system. 

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_53d05e68)

---

## My first terminal commands

The first command I ran for this project is cd ~/Desktop/DevOps


I also updated my private key's permissions by running a change mode command using terminal "chmod 400" 

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_9328ada1)

---

## SSH connection to EC2 instance

To connect to my CE2 instance I, ran the commandssh -i ~/Desktop/DevOps/Github.pem ec2-user@ec2-100-27-28-149.compute-1.amazonaws.com

### This command required an IPv4 address

A server's IPv4 DNS is what the internet will use to locate my EC2 instance.

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_e3069dca)

---

## Maven & Java

Apache Maven is a tool the helps devs organize Java Projects it also works as a package manager. 

Maven is required for this project because it will help get the ball rolling on my current project by provifing templates for startes. 

Java is a commly used programming language that can buil danything from mobile apps to enterprise level systems. 

Java is required for this project because with out it we would not be able to run Maven 

---

## Create the Application

I generated a Java web app using the command 

mvn archetype:generate    -DgroupId=com.nextwork.app    -DartifactId=nextwork-web-project    -DarchetypeArtifactId=maven-archetype-webapp    -DinteractiveMode=false

I installed remote - SSH, which is an extension inside of VS code. I installed it to unlock Vs codes IDE features 

Configuration details required to set up a remote connection include the hostname of the EC2 instance, the file location of the Private key and the username 

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_2939cf01)

---

## Create the Application

Using VS Code's file explorer, I could see all of the files and folders I've created with Maven and the web app 

Two of the project folders created by Maven are src and webapp, which hold all the source code files that define how the webapp looks and the web apps files and resources. 

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_45f91fd7)

---

## Using Remote - SSH

index.jsp is a file used in Java web apps. It's similar to an HTML file because it contains markup to display web pages.However, index.jsp can also include Java code, which lets it generate dynamic content.

I edited index.jsp by changing the place holder code to something more personal.

![Image](http://learn.nextwork.org/motivated_turquoise_jolly_newt/uploads/aws-devops-vscode_7a1de541)

---

## Using nano

---

---

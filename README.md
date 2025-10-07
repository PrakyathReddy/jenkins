# jenkins

#### steps to setup jenkins on ec2 server

1. launch ec2 instance on AWS and ssh into it
2. install java JDK - <br>
   $ sudo apt update <br>
   $ sudo apt install fontconfig openjdk-21-jre <br>
   $ java -version <br>
3. install jenkins <br>
   $ sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key <br>
   $ echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null <br>
4. edit inbound rules on the security group attached to ec2 instance to allow traffic on port 8080 which is where jenkins runs 
5. take the public ip of ec2 instance and access through any browser using port 8080

![install](installation-complete.png)


# jenkins

#### steps to setup jenkins on ec2 server

1. Launch ec2 instance on AWS and ssh into it
2. install java JDK - 
   $ sudo apt update
   $ sudo apt install fontconfig openjdk-21-jre
   $ java -version
3. install jenkins
   $ sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
   $ echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
4. 
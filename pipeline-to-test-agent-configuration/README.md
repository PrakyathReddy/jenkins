configuring docker as agent and verifying if the container has nodejs or not, because i have used a nodejs container

jenkins will request docker to spin up a container on the fly, and assign the job to it, then terminate the container once the job is complete.

On jenkins: 

new item > pipeline > pipeline script from scm > update repo url & branch name > provide path to jenkinsfile on repo
Click Build Now

Steps followed by jenkins can be seen in the console
1. git repo cloned
2. checked if docker container specified as agent exists or not
3. created docker container to run agent
4. command mentioned in 'test' stage executed
5. docker container terminated after job was completed
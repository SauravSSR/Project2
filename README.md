<h1> Jenkins Installation in Ubuntu </h1>
<h2> Installation </h2>

- Step 1: First add the key to your system.

    sudo curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee \
    /usr/share/keyrings/jenkins-keyring.asc > /dev/null

- Step 2: Add a Jenkins apt repository entry.

   sudo echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
   https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
   /etc/apt/sources.list.d/jenkins.list > /dev/null

-  Step 3: Update your local package index
   sudo apt-get update

- Step 4: Install Java

  sudo apt-get install fontconfig openjdk-11-jre

- Step 5: Install Jenkins

 sudo apt-get install jenkins
   
<h2> Checking for Jenkins </h2>.

  jenkins --version
   
<h2>Start Jenkins</h2>

- Step 1: Enable the Jenkins service to start

  sudo systemctl enable jenkins
- Step 2: Start the Jenkins service
   sudo systemctl start jenkins
- Step 3: Check the status of the Jenkins service
   sudo systemctl status jenkins
   
<h2> Unlocking Jenkins </h2>
- Step 1: Browse to http://<localhost>:8080
   /var/lib/jenkins/secrets/initialAdminPassword
   will be displayed
- Step 2: Go back to terminal and type cmd
   sudo cat /var/lib/jenkins/secrets/initialAdminPassword
   copy the password displayed
- Step 3: Go back to the browser and paste the password
   and begin Jenkins installation
   
<h1> Docker Installation in Ubuntu </h1>

<h2> Installation </h2>
- Step 1: Update your local package index
   sudo apt-get update
- Step 2: Install Docker
   sudo apt install docker.io -y
   
<h2> Check for Docker </h2>
   docker --version

  
<h1> Git Installation </h1>
<h2> Install Git </h2> 
   sudo apt install git
<h2> Check Git </h2>
   git version
  

# Practice
 	 
 
     
 
 
Continuous Integration/Continuous Delivery 
Course code: 21CD311 
 
 
B.Tech (Devops ) – 5st Sem & 3st Year 
In 
Computer Science  
 
Under the Supervision of 
Mr. Sandeep Dalal 
 Assistant Professor 
 
By 
Anuj Pal 
11722210019 
Class A309 Sec F 
 
 
Department of Computer Science 
SRM University, Sonipat 
Haryana, 131028 
 
 
 
 
INDEX 
 
S. 
No. 
 	List of Content 	 
 
Page No. 	Signature 
1. 	Introduction to Jenkins and setup/configuration 
 	 
 	 
2 	 Installing Java and Jenkins 
Using Ubuntu in Command 
Prompt 	 
 	 
3 	How to install Jenkins 
using .WAR file 
 	 	 
4 	Linking VScode and GitHub . 
 	 	 
5 	Creating a freestyle Jobs in Jenkins. 	 	 
6 	TO CREATE A 
FREESTYLE JOB WITH 
PARAMETERS 	 	 
7 	TO CREATE A 
FREESTYLE JOB WITH 
GITHUB 	 	 
8 
 	To integrate Git with Jenkins by installing  plugins and specifying path in Jenkins. 	 	 
 	 
 
9 	To install plugins manually in Jenkins. 
 	 	 
10 	To build and test pipeline script in Jenkins. 
 	 	 
11 	Use Jenkins as a Continuous Integration Server. 
 	 	 
12 	Backup Management in Jenkins Server. 	 	 
13 	To build a ci/cd pipeline for Java application using maven. 	 	 
14 	To build a freestyle project using maven for java application. 	 	 
 
Practical -1 
Introduction to Jenkins and setup/configuration 
 
1- Jenkins 
 
What is Jenkins? 
Jenkins is an open-source automation server used primarily for continuous integration (CI) and continuous delivery (CD). It helps automate various aspects of software development, such as building, testing, and deploying code. Jenkins supports various plugins that integrate with different tools and services, making it highly customizable and adaptable to various workflows. 
 
Why Jenkins is needed? 
Jenkins is commonly used in DevOps practices to streamline the development process and ensure consistent and reliable delivery of software. 
 
 
 
2- Setup/Configuration 
 
Step-by-Step Guide to Download and Install Java JDK 1. Choose the JDK Version 
Before downloading, decide which version of the JDK you want to install. The latest Long-Term Support (LTS) version is JDK 17, but JDK 11 is also widely used. 
 
2. Download the JDK 
Visit the Oracle JDK Download Page: 
o	Go to the Oracle JDK Downloads page Select the JDK Version: 
o	Select the JDK 21 version as the newer JDK 22 version is not supported by the Jenkins. 
 
 
Download the Windows Installer: 
o	Scroll down to the section titled "Windows" and download the .exe installer (e.g., jdk-17_windows-x64_bin.exe). 
 
 
 
 
 
Install the JDK 
Run the Installer: 
o	Double-click the downloaded .exe file to start the installation. 
Follow the Installation Wizard: 
o	Click "Next" to proceed through the installation steps. 
o	By default, the JDK is installed in C:\Program Files\Java\jdk-21 (or the version you downloaded). You can change the installation path if needed. 
Complete the Installation: 
o	Once the installation is complete, click "Close" to exit the installer. 
  
 
 
Step-by-Step Guide to Download and Install Jenkins 
1.	Download Jenkins 
•	Visit the Jenkins Download Page: 
o	Go to the official Jenkins download page. 
•	Download the Jenkins Windows Installer: 
o	Under the "Windows" section, click on the link to download the "Jenkins Windows Installer" (a .msi file). It will look something like jenkins.msi. 
 
 
2.	Install Jenkins 
•	Run the Installer: 
o	Once the download is complete, double-click the .msi file to start the installation process. 
•	Follow the Installation Wizard: 
o	Click Next on the welcome screen. o Accept the license agreement and click Next. 
o	Choose the installation directory or accept the default (C:\Program Files (x86)\Jenkins) and click Next. 
o	Click Install to begin the installation. The installer will set up Jenkins as a service and install it. 
 
 
 
 
                                                                                         	                  
 	 
 
 
 
 
 
Installing Jenkins now 
 
  
 
 
 
1.	Access Jenkins 
•	Open Jenkins in Your Browser:
o	Open your web browser and go to http://localhost:8080. This is the default address for Jenkins. 
•	Unlock Jenkins:
o	The first time you access Jenkins, it will ask for an initial admin password. This password is located in a file on your system. 
 
 
 
•	Find the Admin Password:
o	Open File Explorer and navigate to C:\Program Files (x86)\Jenkins\secrets. 
o	Open the file named initialAdminPassword with a text editor like Notepad. Copy the password from this file. 
 
 
•	Enter the Admin Password:
o	Paste the password into the Jenkins setup screen and click Continue. 
 
 
 
2.	Set Up Jenkins 
•	Install Suggested Plugins:
o	Jenkins will prompt you to install plugins. Select Install suggested plugins to install the most commonly used plugins. 
•	Create an Admin User:
o	After the plugins are installed, Jenkins will prompt you to set up your first admin user. Fill in the necessary details and click Save and Finish. 
•	Start Using Jenkins:
o	Once the setup is complete, you will be redirected to the Jenkins dashboard. You can now start creating jobs and pipelines. 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
3.	The final process of the setup id to sign up by inputting your credentials 
 
 
 
 
 
 
 
 
 
 
4.	Jenkins dashboard will be visible like this after logging in 
 
 
 
 
 
 
 
 
 
 	 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
                      
                    Experiment-2 How to install Jenkins using .WAR file 
 
To download and run Jenkins using the `.war` file on Windows, follow these steps: 
 
### Step 1: Download Jenkins WAR File 
 
1.	Go to the Jenkins official website  https://www.jenkins.io/download/ 
2.	Under **Generic Java Package (war)**, click on the **Download** button to download the `.war` file. 
 
  
 
### Step 2: Install Java (if not already installed) 
 
1.	Jenkins runs on Java, so you need to have **Java JDK** installed. 
2.	To check if you have Java installed, open the **Command Prompt** and run: 
 
 
  
 
   If it returns a version, Java is installed. If not, download and install the  **JDK** from the [Oracle website] https://www.oracle.com/java/technologies/downloads/ or use OpenJDK. 
 
 
  
 
 
3.	After installing Java, ensure that the `JAVA_HOME` environment variable is set. You can do this by following: 
-	Right-click on **This PC** → **Properties** → **Advanced system settings**.    - Click on **Environment Variables**. 
-	Under **System Variables**, click **New** and add: 
-	**Variable name**: `JAVA_HOME` 
-	**Variable value**: Path to your Java installation, e.g., `C:\Program Files\Java\jdk-21`. 
 
 
 
  
 
 
 
 
### Step 3: Run Jenkins Using the WAR File 
 
1.	Open **Command Prompt** and navigate to the directory where you downloaded the `jenkins.war` file. You can use the `cd` command, for example: 
 
  
 
2.	Run the Jenkins WAR file using the following command: 
 
  
 
3.	Jenkins will now start up. Once started, it will be available at:      `http://localhost:8080` 
  
 
 
 
 
 
 
### Step 4: Unlock Jenkins 
 
1. After starting Jenkins, open your browser and go to `http://localhost:8080`. 2. You will see an **Unlock Jenkins** screen, asking for the Administrator password. 
3.	To find the password, go back to the Command Prompt where Jenkins is running. It will display something like: 
 
  
 
 
4.	Copy the password and paste it into the **Unlock Jenkins** page. 
 
  
 
 
 
### Step 5: Install Suggested Plugins 
 
1.	Once Jenkins is unlocked, you’ll be asked to install plugins. 
2.	You can choose to **Install suggested plugins** or select specific plugins based on your needs. 
 
  
 
 
### Step 6: Create Admin User 
 
1.	After installing plugins, you’ll be prompted to create your first admin user. 
2.	Fill in the details to create the user. 
 
 
 
  
 
 
### Step 7: Jenkins is Ready 
 
1.	After setting up the admin user, Jenkins will be ready to use! 
2.	You can now access the Jenkins dashboard at `http://localhost:8080`. 
 
 
  
 
By following these steps, you can run Jenkins on Windows using the `.war` file! Let me know if you face any issues during the setup. 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
     
 Experiment-3 
How to install Ubuntu and Jenkins using CMD in Windows 
 
To download and install Ubuntu using the Windows Subsystem for Linux (WSL) command, follow these steps: 
1.	Enable WSL: 
•	Open the Windows Terminal or Command Prompt. • 	Run the following command to enable WSL features: Bash 
wsl --install 
•	This command will install the WSL components and restart your computer. 
 
2.	Download Ubuntu: 
•	Run the following command to download the Ubuntu distribution: Bash 
wsl --install -d Ubuntu 
•	This will download and install the Ubuntu distribution. 
 
  
 
3.	Launch Ubuntu: 
•	After the installation is complete, you can launch the Ubuntu distribution in the Windows Terminal by running: Bash wsl -d Ubuntu 
•	This will open a Ubuntu shell within the Windows Terminal. 
  
 
 
 
 
This guide will help you install Jenkins on an Ubuntu 22.04 system. 
 
Step 1: Install Java 
Jenkins requires the Java Runtime Environment (JRE). This guide uses OpenJDK for the Java environment. OpenJDK is a Development Kit, and includes the Java Runtime Environment. 
At the time of writing this article, Jenkins only supports Java 8 and Java 11 on Ubuntu. You can have multiple versions of Java installed on Ubuntu. If you do, make sure Java 8 or Java 11 is set as the default version. 
Follow the steps below to install Java on Ubuntu: 
1.	Check if you already have Java installed on your Ubuntu system: 
 
Java -version 
 
  
Since Java is not installed on our system, we will install it using OpenJDK. 
 
 
 
 
 
2.	First, open a terminal window and update the system package repository by running: 
    Sudo apt update 
 
Enter your administrator password and wait for the update to complete. 
3.	Depending on which Java version you want to install, Java 8 or 11, run one of the following commands: 
• 	To install OpenJDK 17, run: sudo apt install openjdk-17-jdk -y 
 
  
Step 2: Install Jenkins 
After setting up the prerequisites, follow the steps below to install Jenkins on Ubuntu: 1. Update the system repository one more time. Updating refreshes the cache and makes the system aware of the new Jenkins repository. 
sudo apt update 
 
2.	Install Jenkins by running: sudo apt install jenkins -y 
 
Wait for the download and installation to complete. 
 
  
 
 
 
3.	To check if Jenkins is installed and running, run the following command: 
sudo systemctl status Jenkins 
 
A bright green entry labelled active (running) should appear in the output, indicating that the service is running. 
 
  
Step 3: Modify Firewall to Allow Jenkins 
Allow Jenkins to communicate by setting up the default UFW firewall. 
1.	Open port 8080 by running the following commands: sudo ufw allow 8080 sudo ufw status 
 
 
  
 
 
If you're using a different firewall application, follow its specific instructions to allow traffic on port 8080. 
2.	If you haven't configured the UFW firewall yet, it displays as inactive. Enable UFW by running: sudo ufw enable 
 
 
  
 
 
 
 
 
 
 
 
 
 
Step 4: Set up Jenkins 
Follow the steps below to set up Jenkins and start using it: 
 
1. Open a web browser, and navigate to your server' IP address. Use the following syntax: 
http://ip_address_or_domain:8080 
 
Use the actual IP address or domain name for the server you're using Jenkins on. For example, if you're running Jenkins locally, use localhost (127.0.0.1): http://localhost:8080 
 
  
A page opens prompting you to Unlock Jenkins. Obtain the required administrator password in the next step. 
2.	Obtain the default Jenkins unlock password by opening the terminal and running the following command: sudo cat /var/lib/jenkins/secrets/initialAdminPassword 
 
  
 
3.	The system returns an alphanumeric code. Enter that code in the Administrator password field and click Continue. 
4.	The setup prompts to either Install suggested plugins or Select plugins to install. It’s fine to simply install the suggested plugins. 
 
  
 
You can always install more plugins later. The system continues the initial Jenkins setup. 
5.	The next step is the Create First Admin User. Enter the credentials you want to use for your Jenkins administrator, then click Save and Continue. 
 
  
 
6.	After this, you should set up the Instance Configuration. This is the preferred network address for this Jenkins installation. Confirm the address you want to use for your server. This is most likely the same address you used to get to this configuration page. 
 
  
 
Once you specify the Jenkins URL, click Save and Finish. 
7.	You should see a page that says Jenkins is ready! Click Start using Jenkins to open the Jenkins dashboard. 
 
  
 
 
 
Conclusion 
You should now have a working installation of Jenkins on your Ubuntu 22.04 system. Next, discover how to setup Jenkins on a Kubernetes cluster. If you are using a different distribution of Linux, we also have a guide on how to install Jenkins od Debian 10, and how to install Jenkins on CentOS. 
 
 
 
 
 
    Experiment-4 
Linking Visual Studio Code and GitHub with Jenkins 
  
Installation and Configuration of Git 
•	Git is a distributed version control system used to track changes in source code during software development.  
•	It allows multiple developers to collaborate on a project, maintaining a complete history of changes and enabling them to work simultaneously without conflicts.  
•	Git stores snapshots of the code, rather than just the changes, making it easy to revert to previous versions or branch off to experiment with new features.  
•	It is widely used because of its efficiency, reliability, and ability to handle both small and large-scale projects. 
 
 
 
   
 
 
 
  
 
 
 
 
 
 
Setting up account on Git VS Code for Connecting to GITHUB. 
 
 
•	git status  
Command used to provide an overview of the current state of the working directory as well as the staging area.  
1.	Untracked:- Files that are in your working directory but not yet tracked by Git. These files are not part of the version control until added.  
2.	Modified:- Files that have been changed but are not yet staged for commit. 
3.	Staged:- Files that have been added to the staging area and are ready to be committed.  
The command used to reach this stage is ‘git add file_name’. 
4.	Committed:- Files committed to the local repository. 
The command used to reach this stage is ‘git commit -m <message>’. 
•	git push origin main 
Command used to commit the code from local to remote repository. 
 
 
  
 
 	 
 
 
 
  
  
 
 
Git Branch 
•	Branching in Git is a process of creating a separate line of development within a project. It allows you to diverge from the main codebase and work on features, fixes, or experiments independently without affecting the main code (often called the "main" or "master" branch). When you're done with your changes, you can merge your branch back into the main branch/repository. 
•	Commands  
1.	git branch 
This command is used to list the branches in our repository 
2.	git branch branch_name 
This command is used to create a new branch of any name.  
3.	git checkout branch_name 
This command is used to exit the current branch and work in another branch specified by the branch name.  
4.	git push origin --delete branch_name 
This command deletes the branch from the remote repository. 
5.	git branch -d branch_name 
 
 
PRACTICAL-5 
 
AIM: Creating a freestyle Jobs in Jenkins. 
Procedure: 
Steps to Create a Freestyle Job in Jenkins: 
1.	Open Jenkins Dashboard: 
• Navigate to your Jenkins instance and log in. 
  
2.	Create a New Item: 
• On the Jenkins dashboard, click on the "New Item" or "New Job" button. 
  
 
3.	Enter Item Name: 
• In the "Enter an item name" field, give your job a name first_job. 
4.	Select Freestyle Project: 
• Choose the option "Freestyle project". 
  
5.	Click OK: 
• Once you've selected the Freestyle project, click the "OK" button. 
  
6.	Add a Description: 
• In the Description box, type: 
                     This is my first job. 
  
 
7.	Configure the Job: 
• You'll be taken to the job configuration page. 
8.	Go to the Build Section: 
• Scroll down to the "Build Steps" section and click on "Add build step". 
9.	Choose Execute Shell: 
• From the dropdown, select "Execute Shell" (or "Execute Windows batch command" if you're on Windows). 
10.	Enter Command: 
• In the command box, type the following command to check the Java version: 
                      java –version 
  
 
 
11.	Save the Job: 
•	Scroll to the bottom and click "Save" to save the configuration. 
  
12.	Build the Job: 
•	Now, go back to the job's dashboard and click on "Build Now" to run the job. 
13.	Check Build Status: 
•	Once the job is triggered, you'll see a build appear in the Build History section on the left side of the dashboard. 
•	You can observe the build status by checking the colored ball next to the build number: 
1. Blue/Green: Success 
      2:  Red: Failure 
  
  
 
14.	Check the Console Output: 
•	Once the job finishes, click on the build number (e.g., #1) in the Build History. 
•	Click on "Console Output" to see the results of the java --version command. 
  
 
 
 
 
 
 
 
 
 
 
 
 
PRACTICAL-6 
 
AIM: Freestyle Job with Parameters. 
 
Steps to Create a Freestyle Job with Parameters in Jenkins: 
1.Open Jenkins Dashboard: 
•	Navigate to your Jenkins instance and log in. 
2.Create a New Item: 
•	On the Jenkins dashboard, click on "New Item" or "New Job" button. 
3.Enter Item Name: 
•	In the "Enter an item name" field, enter the name of the job: secondjobwithparameters. 
4.Select Freestyle Project: 
•	Select "Freestyle project" from the options. 
  
5.Click OK: 
•	Once you've selected the Freestyle project, click "OK". 
6.Add a Description: 
•	In the Description box, type: 
                      This is my second job with parameter. 
  
7.Enable Parameterized Build: 
•	Scroll down to the "General" section. 
•	Check the checkbox "This project is parameterized". 
8.Add First String Parameter: 
•	Click on "Add Parameter" and select "String Parameter". • In the Name field, enter: first_name. 
•	In the Default Value field, enter: Anuj 
•	In the Description field, enter: User's_firstname. 
  
 
 
9.Add Second String Parameter: 
•	Click on "Add Parameter" again and select "String Parameter". 
•	In the Name field, enter: last_name.  
•	Leave the Default Value blank (if you prefer) or add a value. 
•	In the Description field, enter: User's_lastname. 
  
10.Add Build Step: 
•	Scroll down to the "Build" section. 
•	Click on "Add build step" and select "Execute Windows batch command" (if you're on Windows) or "Execute shell" (if you're on Linux/Mac). 
•	In the command box, write the following for Windows: 
1.	@echo %first_name% %last_name% 
11.Save the Job: 
•	Scroll to the bottom and click "Save" to save the job configuration. 
  
12.Run the Job: 
•	Go back to the job’s dashboard. 
•	Click on "Build with Parameters". 
•	Provide values for first_name and last_name (or use the default for first_name), and click "Build". 
 
13.Check Build Status: 
•	Once the job is triggered, you'll see a build appear in the Build History section on the left side of the dashboard. 
•	You can observe the build status by checking the colored ball next to the build number: 
1.	Blue/Gree 
2.	Red: Failure 
  
14.Check the Console Output: 
•	Once the job is complete, click on the build number (e.g., #1) in the Build History. 
•	Click on "Console Output" to see the result, where it should display the first_name and last_name as provided. 
  
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
PRACTICAL-7 
 
AIM: Configuring Jenkins with Git Plugin. 
Procedure: 
Step 1: Install the Git Plugin in Jenkins: 
1.	Access Jenkins Dashboard: 
•	Open Jenkins in your browser and log in. 
 
  
2.	Navigate to Manage Jenkins: 
•	From the dashboard, go to Manage Jenkins > Manage Plugins. 
  
  
3.	Install the Git Plugin: 
•	In the Available tab, search for Git Plugin. 
•	Select it and click Install without restart. Wait for the installation to complete. 
  
Step 2: Configure Global Git Settings: 
1.	Go to Global Tool Configuration: 
•	From the dashboard, go to Manage Jenkins > Global Tool Configuration. 
 
  
2.	Add Git Executable Path: 
•	Under the Git section, click Add Git. 
•	Name your Git installation (e.g., Default Git) and specify the Path to Git executable if it’s not installed in the default location. 
•	Click Save. 
  
 
 
 
 
 
 
PRACTICAL-8 
 
AIM:   Freestyle job with GitHub. 
Procedure: 
Steps to Create a Freestyle Job with GitHub and View Build Output: 
1.	Open Jenkins Dashboard: 
• Navigate to your Jenkins instance and log in. 
2.	Create a New Item: 
• On the Jenkins dashboard, click on "New Item". 
3.	Enter Item Name: 
• In the "Enter an item name" field, type: job-3_SetupWithGithub. 
4.	Select Freestyle Project: 
• Choose "Freestyle project". 
5.	Click OK: 
• After selecting the Freestyle project, click "OK". 
  
6.	Add Description: 
• In the "Description" box, type: 
                      This is my 3rd job with GitHub. 
  
7.	Open GitHub and Copy Repository URL: 
•	Go to your GitHub repository, for example: https://github.com/yourusername/your-repo-name. 
•	Copy the URL of the repository (make sure to copy the HTTPS or SSH URL, depending on your setup). 
  
8.	Enable GitHub Project in Jenkins: 
•	In the General section of Jenkins, check the box "GitHub project". 
•	In the Project URL field, paste the GitHub repository URL you copied earlier (e.g., https://github.com/your-username/your-repo-name). 
  
9.	Configure Source Code Management (SCM): 
•	Scroll down to the Source Code Management (SCM) section. 
•	Select "Git". 
•	In the Repository URL field, paste the GitHub repository URL (e.g., https://github.com/your-username/your-repo-name.git). 
•	If your repository is private, make sure to add and select the proper Credentials (GitHub username/password or personal access token). 
  
10.	Modify Branches to Build: 
•	In the Branches to build section, remove the default main or master branch. 
•	If you want to build a specific branch, enter its name (e.g., feature-branch). If not, leave it blank for now. 
11.	Save the Job: 
• Scroll to the bottom and click "Save" to save the job configuration. 
  
Steps to Build and Check Console Output: 
1.	Run the Job: 
•	Go back to the job’s dashboard. 
•	Click on "Build Now" to trigger the job. 
  
 
2.	Check Build Status: 
•	Once the job is triggered, you'll see a build appear in the Build History section on the left side of the dashboard. 
•	You can observe the build status by checking the colored ball next to the build number: 
1.	Blue/Green: Success 
2.	Red: Failure 
3.	View Console Output: 
•	After the build finishes, click on the build number (e.g., #1) under Build History. 
•	Click on "Console Output" to see the detailed log. 
•	Look for the message: "Building in workspace" followed by a file path (C:\Program Files\Jenkins\workspace\job-3_SetupWithGithub). 
 
  
4.	Copy Workspace URL: 
•	From the Console Output, copy the file path where Jenkins has built the project. This will be shown after the text "Building in workspace". 
5.	Open Workspace in File Explorer: 
•	Open File Explorer (on Windows) or your file manager. 
•	Paste the copied URL from the Jenkins console output into the address bar of File Explorer and press Enter. 
•	You should now see the contents of the repository Jenkins has cloned, including the README.md file. 
  
 
6.	Open the README File: 
•	Find the README.md file in the repository folder. 
•	Double-click to open the file and view its content. 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
PRACTICAL-9 
 
AIM: Adding the Plugin manually to Jenkins. 
Procedure: 
Step 1: Download the Plugin 
•	Go to the Jenkins Plugin Index https://updates.jenkins.io/download/plugins/ 
 
  
•	Search for the plugin you need. 
  
•	Download the .hpi or .jpi file of the plugin from the plugin page. 
 
 
  
Step 2: Upload the Plugin in Jenkins • Open your Jenkins dashboard. 
  
•	Go to Manage Jenkins > Manage Plugins. 
  
•	Switch to the Advanced tab. 
  
•	In the Upload Plugin section, click on Choose File and select the downloaded .hpi or 
.jpi file. 
  
 
•	Click on Upload to install the plugin. 
  
Step 3: Restart Jenkins 
•	Some plugins may require a restart to activate. After installation, you may see an option to restart Jenkins. 
Step 4: Verify Plugin Installation 
•	After the restart, go back to Manage Plugins > Installed and check if the plugin appears in the list. 
  
 
 
 
 
 
 
 
 
 
PRACTICAL-10 
 
AIM: Creating Jenkins pipeline with pipeline script. 
Procedure: 
Steps to Create a Jenkins Pipeline with a Pipeline Script: 
Step 1: Configure the Pipeline in Jenkins 
1.	Go to Jenkins Dashboard > Click on New Item > Enter the project name and select Pipeline. 
  
2.	Write the description and scroll down to the Pipeline section. 
  
3.	Under Definition, select Pipeline script HelloWorld and write script for Build, Test and Deploy Stages. 
  
4.	Save the configuration. 
  
Step 2: Run the Pipeline After configuration: 
1.	Click Build Now to start the pipeline. 
  
2.	Monitor the stages from the pipeline view. 
 
  
3.	Stages of the pipeline. 
  
4.	Console Output of the pipeline. 
  
 
 
Step 3: Do some changes in the pipeline script and monitors the error in it. 
  
1.	Console Output is showing the error. 
  
2.	Stages of the pipeline. 
  
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
                                       EXPERIMENT-11 
USE JENKINS AS A CONTINUOUS INTEGRATION SERVER 
Continuous integration with Jenkins 
A Three Part Process: The CI workflow described in this article is composed of three steps. The developer first pushes a commit to GitHub, which in turn uses a webhook to notify Jenkins of the update. Jenkins can then pull the GitHub repository, build the Docker container which contains our stack and then run the test. If the test passes,  Jenkins will push the code to the master branch. 
 
Before we conclude this chapter, here is a list of the key practices of Continuous Integration(as defined by Martin Fowler in 2006) with the examples of the ways in which Jenkins can be used to help you achieve them: 
•	Maintain a Single Source Repository: Jenkins can interact with all the modern source code and version control repositories- some abilities are builtin, others can be added as extensions. 
•	Automate the Build: As described earlier in the use cases, this is one of the core aims of Jenkins and often the main driver to start using Jenkins. 
•	Make Your Build Self-Testing: This is usually the second step in setting up a CI environment with Jenkins- once you automate the building of the code, automating the tests as well is a natural progression. 
•	Everyone Commits To The Mainline Every Day: We can’t really force developers to do this unfortunately. However, we can quite easily highlight and report who is doing-or not doing-what, which should eventually help them learn to follow this best practice. 
•	Every Commit Should Build the mainline on an Integration Machine: 
Builds can be triggered by developer commits, and Jenkins Slave Nodes can be used to build and provide accurate replica environments to build upon. 
•	Fix Broken Builds Immediately: This is another developer best practice that needs to be adopted- when Jenkins shows red, the top focus should be on fixing the issue until it shows green. No one should commit new changes while the build is broken, and Jenkins can be configured to communicate the current status in the most effective way. 
•	Keep the Build Fast: By offloading and spreading work to distributed Slave Nodes and by breaking down builds to identify and focus on the areas that have changed, Jenkins can be turned to provide a rapid response to changes- a good target would be to check in a change and obtain a clear and obtain a clear indication of the result or impact under 10 minutes. 
•	Test in a Clone of the Production Environment: After compiling the new change, downstream Jenkins jobs can be created that will prepare the environment and take it to the required level- applying database changes, starting up dependent processes, and deploying other prerequisites. Using virtual machines or containers in conjunction with Jenkins to automatically start up environments in a known-good state can be very useful here. 
•	Make it Easy for Anyone to Get the Latest Executable: Jenkins can be set up to act as a web server hosting the latest version at a known location so that everyone (and other processes/consumers) can easily fetch it, or it can also be used to send out details and links to interested parties whenever a new version has been uploaded to Nexus, Artifactory, and so on. 
•	Everyone can see what’s happening: There are many ways in which Jenkins communications can be extended- email alerts, desktop notifications, Information Radiation, RSS feeds, Instant Messaging, and many more- from lava lamps and traffic lights to the ubiquitous toy rocket launchers! 
•	Automate Deployments:  This is usually a connect to the target and update it with the most recently build artifact.gical progression of the Build->Test>Deploy automation sequence, and Jenkins can help in many ways; with Slave Nodes running on the deployment host, or jobs set up. 
CONCLUSION: In summary, Jenkins is a robust tool for implementing Continuous Integration (CI), automating processes from code building to testing and deployment. By adhering to best practices, Jenkins enables teams to maintain a central code repository, automate builds and tests, and receive quick feedback on changes.  
 
 
 
 
 
 
 
 
EXPERIMENT – 12 
BACKUP MANAGEMENT IN JENKINS SERVER 
 
AIM: To download backup plugins for backup management in Jenkins. 
THEORY: 
ThinBackup is a popular Jenkins plugin used for creating backups of Jenkins configurations, job data, and other important files. It’s particularly useful for administrators who want a straightforward, lightweight backup solution for Jenkins, as it allows them to automate and schedule backups without manual intervention. 
PROCEDURE: 
Below are the step-by-step instructions on how to set it up: Step 1: Click on Manage Jenkins and then go to Plugins. 
 
Step 2: Now click on Available plugins and then search for ThinBackup (plugin for backup management in Jenkins). 
 
Step 3: Then after successfully installing the plugin restart the Jenkins. 
 
Step 4: Now to check whether the plugin is installed or not we will click on Installed Plugins and search for ThinBackup. 
 
Step 5: Now click on Manage Jenkins and then go to System and then search for ThinBackup in it and make a new folder and enter its path in the ThinBackup part. 
 
 
 
Step 7: When we again go to the folder we observe that various files are already automated. 
 
CONCLUSION: We have successfully downloaded ThinBackup (a plugin used for backup management in Jenkins). 
EXPERIMENT – 13 
Maven integration with Jenkins 
 
AIM – To setup maven with Jenkins for java application. 
 
This document explains the process of integrating Maven with Jenkins by using a random project from GitHub. It covers the steps from setting up Jenkins, installing necessary plugins, configuring Maven, and building a project through a pipeline or freestyle project. 
 
PROCEDURE: 
Step 1: Select a random maven project from github and copy that project’s URL. 
  
 
Step 2: In Jenkins, click on new item, create a new freestyle project named “maven-demo”. 
  
 
Step 3: Click on Git & paste the Git-hub repository URL in Repository URL and save and check the branch specified in the chosen project.  
  
 
 
  
 
 
Step 4: Click on Build Now to start building the project. 
  
The build is successful. 
  
 
Step 5: Go to manage Jenkins, then plugins and under available plugins, search for “Maven Integration” plugin and install it. 
  
 
Step 6: Now, go to Manage Jenkins, then Tools, then click on Add Maven and fill the required information as shown below and save.   
  
Step 7: In the Configuration section, select Invoke top-level Maven targets in the Build Steps. 
  
 
Step 8: Select Jenkins-maven in Maven version. 
  
 
Step 9: In the Git-hub repo, open Jenkins file. 
  
Step 10: In Build stage, copy the selected command. 
  
 
Step 11: Now, paste the selected command in Goals. 
  
 
Hence, as shown the build is successful.  
  
  
 
CONCLUSION: 
By following this step-by-step guide, you can successfully integrate 
Maven with Jenkins to build a project from GitHub. Whether using a Freestyle Project or a Pipeline Job, Jenkins enables you to automate your build, test, and deployment processes with ease. 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
                                EXPERIMENT – 14 
CI/CD Pipeline for Java Application 
 
AIM – To build a ci/cd pipeline for Java application using maven. 
 
INTRODUCTION: 
This document provides a step-by-step guide on how to build a CI/CD pipeline for a Java application using Maven and Jenkins. The pipeline will automate the process of building, testing, and deploying a Mavenbased Java application. Continuous Integration (CI) and Continuous Deployment (CD) ensure that changes made to the codebase are automatically built, tested, and deployed in a consistent manner. 
 
PROCEDURE: 
Step 1: Create a new pipeline project named “maven-pipeline”. 
  
 
Step 2: Copy the https link of java application repository available from Git-hub and paste the URL under project URL. 
  
Step 3: In Advanced Project Options, and Pipeline script select GitHub + Maven. 
  
 
 
Step 4: Change the script as follows: 
  
  
 
Step 5: Hence, all stages of pipeline has succeeded. 
  
 
CONCLUSION:  
Hence, we have successfully built a ci/cd pipeline for our maven project. 
 
 
                                                                                         	                  
 	 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 

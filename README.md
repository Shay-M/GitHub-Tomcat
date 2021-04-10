# GitHub-Tomcat

Monitoring Task
 Installing tomcat on windows:
Please Note ! 
Tomcat doesn’t work without java, so before installing tomcat on the machine, you should install a compatible java runtime version and setup JAVA_HOME environment variable.
Installation :
    • Download the windows service installer from here.
    • Install the downloaded file, pass all the setup until reaching Configuration Options:


To change the default running port of tomcat, open “server.xml”
under conf folder and change the port attribute of Connector tag.


Git configuration:
Create new repo in GitHub - tomcat application
In your text editor, you will develop a simple JSP that creates a web page. 
Add (add-> commit -> push) the Date.jsp file (choose from web or create new) to your new repository . 
Jenkins configuration:
Ensure plugin - GitHub integration is installed
1.Create new job
2.Configure which Git Repositories to work with the jenkins:
3.Configure Build Triggers.
(the Jenkins job automatically pull the files from repo) 
Execute windows command:
    • Build -> Add build step -> Execute windows batch command -> create directory under your CATALINA_HOME/webapps/ROOT with your name (i.e c:/Program Files/Apache Software Foundation/Tomcat8.5/webapps/ROOT/Ziv_Vilozni)
    • Build -> Add build step -> Execute windows batch command -> Copy your file to the new path
Monitoring stage:
    • Download monitor plugin from jenkins.
    •  Add monitor stage (in build stage or post build) to your Job (test your URL)
Jenkins with Git:
    1. Change the JSP file in Git, verify the new change.
    2. Produce  a failure in your test
Finished– Great!!!


    1. Take a screenshot of your GITHUB Repository (showing your name)
    2. Take a screenshot of your Jenkins Job (with success)  and Jenkins Job 
Configuration.
    3. Take a screenshot of your Tomcat website (showing your URL)
    4. Take a screenshot with the results from monitor (showing success and after the change with failure)
    5. Upload to Moodle

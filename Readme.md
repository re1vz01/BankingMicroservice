Capstone Project -DevOps
ABC is Software Company currently following Agile Methodology for one of the Banking client and most of the SDLC steps are manual. Client is migrating the applications into microservices and restapi.Now client wants to automate project using CI/CD pipeline.

CI/CD pipeline using jenkins
Git Requirement
The project is maven based microservice, which has a main file App.java.
This project has a unit test program that is available in src/test/ folder
The changes to these files should be tracked and Code Reviewer should review all the changes.
Create a GitHub Repository BankingMicroservice.
On this project there are multiple developers are working so as a Code reviewer create each branch for each developer and once they finish their development then they push the code to their own branch and you have to review the code and merge it into Master branch (A branch which has the latest code)
Build Automation is part of CI/CD pipeline.
You should record all the commits into local repository and once the changes are done it should be pushed to Remote GitHub Repository BankingMicroservice.
On Remote Repository Create a Readme.md file which is documentation of your project.
Maven Requirement
Code should be built Automatically as soon as Master branch for BankingMicroservice is updated.
Required dependencies should be automatically added (In this case junit framework should be added automatically)
There must be a jar file to be created under the target folder.
Docker requirement
Create a Docker file in BankingMicroservice Repository.
Whenever there is any change that happens in the source code then a new docker image is to be created.
Creation of Docker image should be created Automatically with a new tag (Hint use docker file)
After the creation of the docker image a new docker container is to be created with the latest docker image
Testing requirement (Dummy job as we did not discuss about Testing)
This job is related to test the application.
Send an Email to Developer
An email is to be sent to the developer if the testing is unstable
Configure Email notification as a part of CI.
Prepare production server (It will be Linux server but it can be Ubuntu or RedHat)
Install java on production servers (Hint use Ansible)
Also, install apache on a production server ( It may be required in the future when this project is enhanced)
Start apache service.
Run docker container in the production
Repeat Docker requirement step again for production machine

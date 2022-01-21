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
Repeat Docker requirement step again for production machine.


Commands
********
 mvn -version
 1325  mvn archetype:generate
 1326  ls
 1327  cd capstone
 1328  ls
 1329  cd src
 1330  ls
 1331  cd test
 1332  ls
 1333  apt-get  update
 1334  java -version
 1335  wget -qO - https://pkg.jenkins.io/debian-stable/jenkins.io.key | apt-key add -
 1336  sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
 1337  sudo apt-get update
 1338  sudo apt-get install jenkins
 1339  systemctl status jenkins
 1340  sudo ufw allow 8080
 1341  vi /etc/sudoers
 1342  git remote add origin git@github.com:re1vz01/BankingMicroservice.git
 1343  git init
 1344  cd ..
 1345  git init
 1346  git remote add origin git@github.com:re1vz01/BankingMicroservice.git
 1347  touch 1.java
 1348  git add .
 1349  git commit -m "1.java is added"
 1350  gitconfig --global user.name Reivin
 1351  git config --global user.name Reivin
 1352  git config --global user.email reivin@gmail.com
 1353  git commit -m "1.java is added"
 1354  ls
 1355  git push origin master
 1356  ssh-keygen
 1357  vi /root/.ssh/id_rsa.pub
 1358  git push origin master
 1359  vi .git/config
 1360  ls
 1361  cat /root.ssh/id_rsa.pub
 1362  cat /root/.ssh/id_rsa.pub
 1363  git push origin master
 1364  vi .git/config
 1365  git branch -m Main
 1366  git push origin master
 1367  git remote add origin git@github.com:re1vz01/BankingMicroservice.git
 1368  vi /root/.ssh/id_rsa.pub
 1369  git push origin master
 1370  ls
 1371  rm 1.java
 1372  ls
 1373  git add .
 1374  git commit -m "Initial commit"
 1375  git push origin master
 1376  git show-ref
 1377  git push -u origin main
 1378  git status
 1379  git add .
 1380  git commit -m "Initial commit"
 1381  git push origin master
 1382  git push -u origin main
 1383  git push origin Main
 1384  git branch dev1
 1385  git branch dev2
 1386  git checkout dev1
 1387  git push origin dev1
 1388  git push origin dev2
 1389  git branch
 1390  ls
 1391  cd /src/test
 1392  ls /src
 1393  ls src/
 1394  ls /src/main
 1395  ls src/main
 1396  vi src/main/java
 1397  cd src/main
 1398  ls
 1399  cat java
 1400  cd java
 1401  ls
 1402  ls capstone/
 1403  cd capstone
 1404  vi App.java
 1405  git checkout dev2
 1406  vi App.java
 1407  git checkout master
 1408  git branch
 1409  git checkout Main
 1410  git merge dev1
 1411  git merge dev2
 1412  git merge dev1 dev2
 1413  git log --oneline


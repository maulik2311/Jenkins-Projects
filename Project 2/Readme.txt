Important:

CI and CD
Automated Deployment on Tomcat web server

How?

On server(Ec2)
1. JAVA11----> amazon-linux-extras java-openjdk11
2. Jenkins --->   on it --> JAVA & MVN (For Source code package)
3. Git   -->  (for conf file (remote repo data))
4. Tom-Cat  -->  Setup 3 things 1.context.xml(To access trafic from anywhere), 2.tomcat-user.xml(Set admin     			password),3.server.xml(Change port number))

Outside server:
5. Need GitHub Repository ----> Source code

Configure all to perform automated deployment

How it work?
Source code(Github)--> Jenkins(Trigger job)--> mvn(package the code)--> Deploy(On TomCat Server)



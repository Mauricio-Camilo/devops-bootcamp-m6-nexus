# Demo Project

Run Nexus on Droplet and Publish Artifact to Nexus

## Technologies Used

- Nexus, DigitalOcean, Linux, Java, Gradle< maven

## Project Description

- Install and configure Nexus from scratch on a cloud server.
- Create new User on Nexus with relevant permissions, and run Nexus with this user.
- Java Gradle Project: Build Jar & Upload to Nexus.
- Java Maven Project: Build Jar & Upload to Nexus.

### Details of project

- Build and push gradle project
  After clonning the repository, a plugin was added in code (apply plugin: 'maven-publish') in order to run the a publish command. The artifact publication and nexus repository were also set, using variables from other files. After these configuration, the application was built and published using gradle publish. The files were verfieid in Nexus browse section.

- Build and push maven project
  Similiar to the gradle project, maven also installed a plugin to upload jar file to nexus, configuring the xml file. In this project, the credentials were set in .m2 folder in a xml file. After the configurations, the comands mvn package and mvn deploy were executed, to build the app and upoad the artifact to nexus.



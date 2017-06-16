# Sample JAVA EE 7
	Author: Khemroat Loem
 	Technologies: JSF, Wildfly (JBoss) as, Maven
 	Summary: This is a quick sample Java EE7. I uses JSF as front-end. I'm using wildfly as application server, you can also use tomcat
 	Target: 

# Requirements
	Make sure you have wildfly 8 or later install in your machine.
	Note: The following snippset from pom.xml file used to enable wildfly deployment with maven command
		<plugin>
			<groupId>org.wildfly.plugins</groupId>
			<artifactId>wildfly-maven-plugin</artifactId>
			<version>1.1.0.Final</version>
		</plugin>
		
	For current version, I'm using H2 database.

## Start application server
	For Windows: ${jboss.home.name}\bin\standalone.bat
	For Linux:   ${jboss.home.name}/bin/standalone.sh
## Build and Deploy
- Make sure the application server is started
- Open a command prompt and navigate to the root directory of the project
- Type the following command

        mvn clean install wildfly:deploy





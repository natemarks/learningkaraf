
#Karaf-command-archetype

When you invoke Apache Maven with the Karaf-command-archetype, a maven-based project will be generated for building a custom Karaf command. Use the following invocation to start the process:

```
mvn archetype:generate \
-DarchetypeGroupId=org.apache.karaf.archetypes \
-DarchetypeArtifactId=karaf-command-archetype \
-DarchetypeVersion=4.0.7 \
-DgroupId=com.your.organization \
-DartifactId=com.your.organization.command \
-Dversion=1.0.0-SNAPSHOT \
-Dpackage=com.minimugs.organization
```

During project generation, you will be prompted to provide the command name, its description, and define in which scope it exists. Once the project is generated, you may then import it into your IDE for further development.

```
[BUNCH OF MAVEN IMPORT STUFF]
Define value for property 'command': : commandNNNAME
Define value for property 'description': : Some crappy command
Define value for property 'scope': : VITCH
Confirm properties configuration:
groupId: com.your.organization
artifactId: com.your.organization.command
version: 1.0.0-SNAPSHOT
package: com.minimugs.organization
command: commandNNNAME
description: Some crappy command
scope: VITCH
 Y: : 
[INFO] ----------------------------------------------------------------------------
[INFO] Using following parameters for creating project from Archetype: karaf-command-archetype:4.0.7
[INFO] ----------------------------------------------------------------------------
[INFO] Parameter: groupId, Value: com.your.organization
[INFO] Parameter: artifactId, Value: com.your.organization.command
[INFO] Parameter: version, Value: 1.0.0-SNAPSHOT
[INFO] Parameter: package, Value: com.minimugs.organization
[INFO] Parameter: packageInPathFormat, Value: com/minimugs/organization
[INFO] Parameter: version, Value: 1.0.0-SNAPSHOT
[INFO] Parameter: package, Value: com.minimugs.organization
[INFO] Parameter: groupId, Value: com.your.organization
[INFO] Parameter: scope, Value: VITCH
[INFO] Parameter: description, Value: Some crappy command
[INFO] Parameter: command, Value: commandNNNAME
[INFO] Parameter: artifactId, Value: com.your.organization.command
[INFO] project created from Archetype in dir: /root/com.your.organization.command
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 03:00 min
[INFO] Finished at: 2016-10-03T07:27:49-04:00
[INFO] Final Memory: 15M/178M
[INFO] ------------------------------------------------------------------------

[root@DEV-NPM-Z5-01 ~]# find com.your.organization.command/
com.your.organization.command/
com.your.organization.command/pom.xml
com.your.organization.command/src
com.your.organization.command/src/main
com.your.organization.command/src/main/java
com.your.organization.command/src/main/java/com
com.your.organization.command/src/main/java/com/minimugs
com.your.organization.command/src/main/java/com/minimugs/organization
com.your.organization.command/src/main/java/com/minimugs/organization/commandNNNAME.java
com.your.organization.command/src/main/resources

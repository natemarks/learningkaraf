
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

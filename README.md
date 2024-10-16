# Maven execution
Create a maven directory: mvn archetype:generate -DgroupId=workshopd6 -DartifactId=workshopd6 -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
Compile the maven xml file: mvn compile
Compile and execute java file: mvn compile exec:java -Dexec.mainClass="workshopd6.App"
Compile the maven xml file and create jar file: mvn package

cd target
java -cp workshopd6-1.0-SNAPSHOT.jar fc.Server 12345 ../../src/cookie_file.txt

Check for jar file directory:
jar tvf workshopd6-1.0-SNAPSHOT.jar
1.Install JAVA (if not already installed)

	https://www.oracle.com/java/technologies/javase-jdk8-downloads.html
	Verify by using javac -version command on your terminal

2.Download and Install Maven(if not already installed)

	https://maven.apache.org/download.cgi
	Installation instructions - https://maven.apache.org/install.html

3.Set environment variables(if not already set)

	JAVA_HOME to point jdk folder (example - C:\Program Files\Java\jdk1.8.0_251)
	PATH to include %JAVA_HOME%\bin and apache-maven\bin (example- C:\apache-maven-3.6.3\bin)

(For reference ----- https://www3.ntu.edu.sg/home/ehchua/programming/howto/Environment_Variables.html)

 
3.Download the mysolution2 folder from https://github.com/Majani-Das/NewCodeSolution as zip

4. Unzip and find mysolution2 folder inside NewCodeSolution-master folder

5. Navigate to the mysolution2 folder in command prompt

5. Run the following command to package the project

	mvn clean dependency:copy-dependencies package

4.Use the below command to run the project

	java -jar target/mysolution2-1.0-jar-with-dependencies.jar {input json file path} {output json file path}

Example:
	java -jar target/mysolution2-1.0-jar-with-dependencies.jar Z:\Input.json Z:\OutputFile.json

5. Open and check the OutputFile.json

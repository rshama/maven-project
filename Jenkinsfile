pipeline {

	agent any
	stages {
		stage ('Build') {
			steps {
				bat 'C:/Users/roshama/Documents/apache-maven-3.5.4/bin/mvn clean package' 
				bat "docker build . -t tomcatwebapp:${env.BUILD_ID}"
			}
		}
	}
}
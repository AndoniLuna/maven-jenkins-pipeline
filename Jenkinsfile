pipeline {
	agent any
	tools {
		maven "Maven 3.9.5"
	}
	stages {
		stage('Build Artifact') {
			steps {
				sh "rm -rf maven-simple"
				sh "git clone https://github.com/pabloariasmora/maven-simple/"
				sh "mvn package -f maven-simple/pom.xml"
			}
		}
	}
}

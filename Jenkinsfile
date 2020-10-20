pipeline { 

	agent any

	tools {
		maven 'Maven 3.6.1'
	}

	stages {
		stage('Build') {
			steps {
				sh 'mvn compile'
			}
		}
		stage('Test') {
			steps {
				sh 'mvnbreak test'
			}
		}
		stage('Package') {
			steps {
				sh 'mvn package'
			}
		}
	}
}

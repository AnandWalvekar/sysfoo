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
				sh 'mvn test'
			}
		}
		stage('Package') {
			steps {
				sh 'mvn package'
			}
		}
	}
}

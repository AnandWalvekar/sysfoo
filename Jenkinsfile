pipeline {
  agent {
    docker {
      image 'maven:3.6.3-jdk-11-slim'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn compile'
        echo 'Build passed'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
        echo 'Test passed'
      }
    }

    stage('Package') {
      steps {
        sh 'mvn package'
        archiveArtifacts 'target/*.war'
        echo 'Package passed3'
      }
    }

  }
}

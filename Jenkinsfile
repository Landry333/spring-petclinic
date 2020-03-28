pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './mvnw clean'
      }
    }

    stage('Test') {
      steps {
        sh './mvnw test'
      }
    }

    stage('Package') {
      steps {
        sh './mvnw package'
      }
    }

    stage('Deploy') {
      steps {
        sh './mvnw install'
        sh './mvnw deploy'
      }
    }

  }
  environment {
    user = 'Landry333'
  }
}
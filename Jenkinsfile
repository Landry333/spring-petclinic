pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './mvnw package'
      }
    }

  }
  environment {
    user = 'Landry333'
  }
}
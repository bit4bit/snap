pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh './bin/build'
      }
    }

    stage('Extract RPM') {
      steps {
        sh './bin/cp'
      }
    }
  }

  post {
    always {
      sh './bin/rmi'
    }
  }
}
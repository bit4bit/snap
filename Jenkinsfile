pipeline {
  agent any

  stages {
    stage('Build') {
      sh './bin/build'
    }

    stage('Extract RPM') {
      sh './bin/cp'
    }
  }

  post {
    always {
      sh './bin/rmi'
    }
  }
}
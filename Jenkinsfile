pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ ./main/PES1UG20CS823.cpp - error'
        echo 'Build Stage Successful'
      }
    }
    stage('Test') {
      steps {
        sh './a.out'
        echo 'Test Stage Successful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployment Successful'
      }
    }
  }
  post {
      failure {
        echo 'Pipeline Failed'
      }
  }
}

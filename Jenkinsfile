pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        echo 'checkout the code'
      }
    }
    stage('compile') {
      steps {
        sh 'cd abc'
      }
    }
    stage('deploy') {
      steps {
        sh 'cd bcd'
      }
    }
    stage('email') {
      steps {
        echo 'completed'
      }
    }
  }
}
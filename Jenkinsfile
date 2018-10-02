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
        echo 'cd abc'
      }
    }
    stage('deploy') {
      steps {
        echo 'cd bcd'
      }
    }
    stage('email') {
      steps {
        echo 'completed'
      }
    }
  }
}

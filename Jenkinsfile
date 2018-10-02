pipeline {
  agent any
  stages {
    stage('checkout') {
      environment {
        test = 'value'
      }
      steps {
        echo 'checkout the code'
        git(url: 'https://github.com/gvsubbareddy/pythonproject.git', changelog: true)
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
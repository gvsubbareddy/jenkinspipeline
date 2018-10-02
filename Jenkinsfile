pipeline {
  agent any
  stages {
    stage('checkout') {
      environment {
        ENV = 'INT'
      }
      steps {
        script {
            if($ENV == 'INT') {
                echo 'checkout the code'
                git(url: 'https://github.com/gvsubbareddy/pythonproject.git', changelog: true)
            } else {
                error 'the application is not  deployed!'
            }
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
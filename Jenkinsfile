pipeline {
  agent any
  environment {
        ENV = 'INT123'
  }
  stages {
    stage('checkout') {
      steps {
        script {
            echo 'checkout the code from $BRANCH_NAME'
            echo "$env.BRANCH_NAME"
            if("${env.ENV}" == "INT") {
                echo 'checkout the code'
                git(url: 'https://github.com/gvsubbareddy/pythonproject.git', changelog: true)
            } else {
                error 'the application is not  deployed!'
            }
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
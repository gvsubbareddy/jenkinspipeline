pipeline {
  agent any
  environment {
        ENV = 'INT123'
  }
  parameters {
         choice(
             choices: 'mkt\nint\npv\ndocker',
             description: 'Deploy to Environment',
             name: 'REQUESTED_ACTION')
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
                echo 'the application is not  deployed!'
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

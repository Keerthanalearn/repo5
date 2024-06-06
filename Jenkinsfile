pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello Build'
      }
    }

    stage('Unit Test') {
      parallel {
        stage('Unit Test') {
          steps {
            echo 'Hello Unit test'
          }
        }

        stage('Integration Test') {
          steps {
            echo 'Hello Integration Test'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Hello Deploy'
      }
    }

  }
}
pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            echo 'Hi'
          }
        }

        stage('developer') {
          steps {
            echo 'developer'
          }
        }

      }
    }

  }
}
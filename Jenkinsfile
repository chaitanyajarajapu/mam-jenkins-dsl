pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'developer'
      }
    }

    stage('Test') {
      steps {
        echo 'Test-Test'
      }
    }

    stage('Publish to Stage') {
      steps {
        echo 'publish to stage'
      }
    }

    stage('Deploy to Dev') {
      parallel {
        stage('Deploy to Staging') {
          steps {
            echo 'deployed to prod'
          }
        }

        stage('Deploy To QA') {
          steps {
            echo 'deployed to QA'
          }
        }

      }
    }

  }
}
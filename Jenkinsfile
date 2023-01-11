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

    stage('Deploy to Staging') {
      steps {
        echo 'deployed to prod'
      }
    }

    stage('Send Email') {
      steps {
        emailext(subject: 'Hi', body: 'Build Complete', attachLog: true, compressLog: true, from: 'chaitanya.ja@gmail.com', saveOutput: true, to: 'sre@admin.com')
      }
    }

  }
}
pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/S4nfs/curriculum-app', branch: 'dev')
      }
    }

    stage('pipeline logs') {
      steps {
        sh 'ls -la'
      }
    }

    stage('docker') {
      steps {
        sh 'docker build -f curriculum-front/Dockerfile .'
      }
    }

  }
}
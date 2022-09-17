pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/S4nfs/curriculum-app', branch: 'dev')
      }
    }

    stage('pipeline logs') {
      parallel {
        stage('pipeline logs') {
          steps {
            sh 'ls -la'
          }
        }

        stage('unit test') {
          steps {
            sh 'cd curriculum-front && npm-i && npm run test:unit'
          }
        }

      }
    }

  }
}
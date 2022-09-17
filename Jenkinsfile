pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/S4nfs/curriculum-app', branch: 'dev')
        sh 'ls -la'
      }
    }

  }
}
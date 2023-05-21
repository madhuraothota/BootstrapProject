pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/madhuraothota/BootstrapProject', branch: 'dev', changelog: true)
      }
    }

    stage('') {
      steps {
        sh 'ls -la'
      }
    }

  }
}
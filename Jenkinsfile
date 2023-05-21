pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/madhuraothota/BootstrapProject', branch: 'dev', changelog: true)
      }
    }

    stage('error') {
      parallel {
        stage('error') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-End Unit Test') {
          steps {
            sh 'cd BootstrapProject && npm i & npm run test:unit'
          }
        }

      }
    }

  }
}
pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/danieldt92/curriculum-app-jenkins-docker', branch: 'dev')
      }
    }

    stage('List Content') {
      parallel {
        stage('List Content') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-End Unit Tests') {
          steps {
            sh 'cd curriculum-front && npm i && npm install --save-dev vue-jest && npm run test:unit'
          }
        }

      }
    }

  }
}
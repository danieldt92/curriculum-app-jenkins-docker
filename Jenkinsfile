pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/danieldt92/curriculum-app-jenkins-docker', branch: 'dev')
      }
    }

    stage('List Content') {
      steps {
        sh 'ls -la'
      }
    }

  }
}
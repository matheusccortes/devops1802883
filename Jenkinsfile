pipeline {
  agent any

  tools {
    nodejs 'NodeJs'
  }

  stages {
    stage('Dependency Installation') {
      steps {
        sh 'npm i'
      }
    }

    stage('Test') {
      steps {
        sh 'npm run test'
      }
    }

    stage('Build') {
      steps {
        sh 'docker-compose build'
      }
    }
  }
}

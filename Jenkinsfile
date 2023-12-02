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
        echo 'E2E Tests'
        sh 'npm run test:e2e'

        echo 'CI Tests'
        sh 'npm run test:ci'
      }
    }
  }
}

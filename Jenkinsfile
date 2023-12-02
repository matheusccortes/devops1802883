pipeline {
  agent any

  tools {
    nodejs '12.22.12'
  }

  stages {
    stage('Dependency Installation') {
      steps {
        sh 'npm i'
      }
    }
  }
}

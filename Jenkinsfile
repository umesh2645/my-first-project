pipeline {
  agent {
    docker { image 'node:latest' }
  }
  stages {
    stage('Install') {
      steps { 'npm install' }
    }

    stage('run') {
      steps { 'ng serve' }
    }
  }
}

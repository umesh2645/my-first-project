pipeline {
  agent {
    docker { image 'node:latest' }
  }
  stages {
    stage('Install') {
      steps { sh 'npm install' }
    }

    stage('Build') {
      steps { sh 'ng build' }
    }

    stage('Run') {
      steps { sh 'ng serve' }
    }
  }
}

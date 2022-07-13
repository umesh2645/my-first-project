pipeline {
  agent { label 'windows' }
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

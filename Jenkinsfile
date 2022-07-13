pipeline {
  agent { label 'master' }
  stage('Checkout Code') {
      steps {
          checkout scm
      }
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

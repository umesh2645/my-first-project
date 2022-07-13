pipeline {
  agent { label 'master' }
  
  stages {
    stage('Checkout Code') {
      steps {
          checkout scm
      }
   }

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

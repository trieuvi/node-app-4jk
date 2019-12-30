pipeline {
  agent any

  tools {nodejs "node"}
  
  stages {
    stage('Clone Git') {
      steps {
        sh 'npm config ls'
        git 'https://github.com/trieuvi/node-app-4jk.git'
      }
    }
    
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
    
    stage('Test') {
      steps {
         sh './script/test'
      }
    }
  }
}

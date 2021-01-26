
pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/astrego/jenkins-test.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh ''
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'npm run test'
      }
    }
  }
}
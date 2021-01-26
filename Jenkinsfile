
pipeline {
  agent any
    
  tools {nodejs "NodeJS"}
    
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
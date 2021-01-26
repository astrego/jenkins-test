pipeline {
  agent any
    
  tools {nodejs "NodeJS"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/astrego/jenkins-test.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm i -g parcel-bundler'
        sh 'npm ci'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }

    stage('Build') {
      steps {
        sh 'npm build'
      }
    }      
  }
}
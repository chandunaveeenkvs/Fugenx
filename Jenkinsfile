pipeline {
  agent {
    node {
      label 'dev'
    }
    
  }
  stages {
    stage('checkout') {
      steps {
        sh ' git pull origin'
      }
    }
    stage('build') {
      steps {
        sh 'mvn compile'
      }
    }
  }
  environment {
    dev = 'test'
  }
}
pipeline {
  agent {
    node {
      label 'maven'
    }
    
  }
  stages {
    stage('DEV') {
      steps {
        sh 'echo "DEV"'
      }
    }
    stage('TEST') {
      steps {
        parallel(
          "AUTO-TEST": {
            sh 'echo "AUTOMATION TESTING"'
            
          },
          "QA-TEST": {
            sh 'echo "QA TEST"'
            
          }
        )
      }
    }
  }
}
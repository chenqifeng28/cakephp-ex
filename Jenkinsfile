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
    stage('UAT') {
      steps {
        sh 'echo "Deploy UAT"'
        echo 'Ready for UAT'
      }
    }
  }
}
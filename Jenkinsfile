pipeline {
  agent any
  stages {
    stage('DEV') {
      steps {
        sh 'echo "DEV"'
      }
    }
    stage('TEST') {
      steps {
        parallel(
          "TEST": {
            sh 'echo "TEST"'
            
          },
          "UAT": {
            sh 'echo "UAT"'
            
          }
        )
      }
    }
  }
}
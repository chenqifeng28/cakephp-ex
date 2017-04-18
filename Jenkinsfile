pipeline {
  agent any
  stages {
    stage('DEV') {
      steps {
        sh 'sh \'oc whoami\''
      }
    }
    stage('TEST') {
      steps {
        sh 'sh \'echo "TEST"\''
      }
    }
  }
}
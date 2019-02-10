pipeline {
  agent any
  stages {
    stage('Date') {
      steps {
        sh 'date'
      }
    }
    stage('Where am I') {
      steps {
        pwd(tmp: true)
      }
    }
  }
}
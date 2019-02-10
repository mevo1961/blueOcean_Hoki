pipeline {
  agent any
  stages {
    stage('Date') {
      parallel {
        stage('Date') {
          steps {
            sh 'date'
          }
        }
        stage('') {
          steps {
            timestamps()
          }
        }
      }
    }
    stage('Where am I') {
      steps {
        dir(path: '/tmp/mevo') {
          sh 'pwd'
        }

      }
    }
  }
}
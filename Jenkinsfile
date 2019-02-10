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
        dir(path: '/home/meinolf/Workspace')
        sh 'pwd'
      }
    }
  }
}
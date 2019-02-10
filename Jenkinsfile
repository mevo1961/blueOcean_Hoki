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
        stage('error') {
          steps {
            timestamps() {
              sh 'date'
            }

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
    stage('Send Mail') {
      steps {
        mail(subject: 'Test email', body: 'This is a test in Jenkins Blue Ocean', to: 'mevo1961@gmail.com', from: 'mevo1961@gmail.com')
      }
    }
  }
}
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
      parallel {
        stage('Where am I') {
          steps {
            dir(path: '/tmp/mevo') {
              sh 'pwd'
            }

          }
        }
        stage('error') {
          steps {
            build(job: 'Test_Job', wait: true)
          }
        }
      }
    }
  }
}
pipeline {
  agent any
  stages {
    stage('Date') {
      steps {
        sh 'date'
      }
    }
    stage('Send mail') {
      steps {
        mail(subject: 'Blu Ocean', body: 'Blue Ocean step Mail has been executed successfully', from: 'jenkins@home', to: 'mevo1961@gmail.com')
      }
    }
  }
}
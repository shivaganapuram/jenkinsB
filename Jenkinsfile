pipeline {
  agent any
  stages {
    stage('initialize') {
      parallel {
        stage('initialize') {
          steps {
            sh 'echo \'hello world\''
          }
        }
        stage('docker start') {
          steps {
            sh 'docker run -it ubuntu /bin/bash '
          }
        }
      }
    }
  }
}
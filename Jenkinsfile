pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('create class file') {
      steps {
        sh 'javac ConsumerInterface.java'
      }
    }

    stage('run') {
      steps {
        sh 'java ConsumerInterface'
      }
    }

  }
}
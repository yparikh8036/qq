pipeline {
  agent any
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
pipeline {
  agent any
  stages {
    stage('simplepipeline') {
      agent any
      steps {
        echo 'Hello World'
      }
    }
    stage('Testing') {
      parallel {
        stage('Java 7') {
          agent {
            docker 'openjdk:7-jdk-alpine'
          }
          steps {
            sh 'java -version'
            sleep(time: 1, unit: 'MINUTES')
          }
        }
        stage('Java 8') {
          agent {
            docker 'openjdk:8-jdk-alpine'
          }
          steps {
            sh 'java -version'
            sleep(time: 2, unit: 'MINUTES')
          }
        }
      }
    }
  }
}
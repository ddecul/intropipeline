pipeline {
  agent any
  stages {
    stage('simplepipeline') {
      steps {
        script {
          pipeline {
            agent any
            
            stages {
              stage('Say Hello') {
                steps {
                  echo 'Hello World!'
                }
              }
            }
          }
        }
        
      }
    }
  }
}
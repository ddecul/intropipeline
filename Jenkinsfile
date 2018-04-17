pipeline {
  agent any
  stages {
    stage('SimpleStep') {
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
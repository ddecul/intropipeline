pipeline {
  agent any
  stages {
    stage('SimpleStep') {
      steps {
        sh '''pipeline {
   agent any
    
   stages {
      stage(\'Say Hello\') {
         steps {
            echo \'Hello World!\'   
         }
      }
   }
}
'''
        }
      }
    }
  }
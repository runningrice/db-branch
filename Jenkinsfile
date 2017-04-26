pipeline {
  agent any
  stages {
    stage('') {
      steps {
        parallel(
          "init0": {
            sh 'echo "init"'
            echo 'i\'m here'
            
          },
          "init": {
            sh 'echo "hello"'
            
          },
          "init3": {
            input(message: 'sss', id: 'aa', ok: 'yes')
            
          }
        )
      }
    }
    stage('test') {
      steps {
        sleep 3
      }
    }
  }
}
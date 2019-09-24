pipeline {
  agent any
  stages {
    stage('BUILD1') {
      parallel {
        stage('BUILD1') {
          steps {
            bat 'echo %Name%'
          }
        }
        stage('BUILD2') {
          steps {
            bat 'echo "This is the second BUILD"'
          }
        }
      }
    }
    stage('TEST1') {
      steps {
        bat 'echo "THIS IS A TEST"'
      }
    }
  }
  environment {
    NAME = 'SIDD'
  }
}
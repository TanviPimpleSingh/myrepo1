pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh 'echo "this is compile step"'
      }
    }
    stage('UnitTest') {
      parallel {
        stage('UnitTest') {
          steps {
            sh 'echo "this is a UnitTest step"'
          }
        }
        stage('UIStep') {
          steps {
            sh 'echo "this is UIstep"'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "this is deploy step"'
      }
    }
  }
}
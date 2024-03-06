pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test parallal'
          }
        }

        stage('Test-Para') {
          steps {
            echo 'test para'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
        sleep 13
      }
    }

  }
}
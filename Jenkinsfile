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
            echo 'hello world'
          }
        }

        stage('test parallal') {
          steps {
            echo 'parallal test step'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
        sleep 13
        sh 'pwd'
      }
    }

  }
}
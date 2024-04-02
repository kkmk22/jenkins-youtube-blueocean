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
            echo 'test'
          }
        }

        stage('test par / print message') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 13
      }
    }

  }
}
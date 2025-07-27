pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date
'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test_pre') {
          steps {
            echo 'test-pro'
          }
        }

      }
    }

    stage('depoly-test') {
      steps {
        echo 'test-time'
      }
    }

    stage('deploy-pro') {
      steps {
        echo 'projection'
      }
    }

  }
}
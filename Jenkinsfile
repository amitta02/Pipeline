pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''date


time'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'This is test '
          }
        }

        stage('error') {
          steps {
            echo 'Unit test '
          }
        }

      }
    }

    stage('current directory') {
      parallel {
        stage('current directory') {
          steps {
            pwd(tmp: true)
          }
        }

        stage('qwe') {
          steps {
            echo 'ok'
          }
        }

      }
    }

    stage('deploy to test') {
      steps {
        echo 'testing env'
      }
    }

    stage('deploy to prod') {
      steps {
        echo 'production'
      }
    }

  }
}
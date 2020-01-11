pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "hey am build stage"'
          }
        }

        stage('build123') {
          steps {
            sh 'echo "build123"'
          }
        }

      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            sh 'echo "how are you"'
          }
        }

        stage('stage1') {
          steps {
            sh 'echo "stage1"'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sh 'echo "this is awesome"'
      }
    }

  }
}
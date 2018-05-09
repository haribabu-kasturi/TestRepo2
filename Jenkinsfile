pipeline {
  agent any
  stages {
    stage('verify') {
      parallel {
        stage('verify') {
          steps {
            echo 'hello'
            echo 'this is the second step'
          }
        }
        stage('docs ') {
          steps {
            echo 'verify docs '
          }
        }
      }
    }
    stage('ABC') {
      steps {
        sh 'echo hello '
      }
    }
    stage('DEF') {
      steps {
        echo 'hello'
      }
    }
    stage('GHI') {
      parallel {
        stage('GHI') {
          steps {
            echo 'mrinmoy'
          }
        }
        stage('BYE1') {
          steps {
            echo 'just before bye'
          }
        }
      }
    }
    stage('END') {
      steps {
        echo 'Complete'
      }
    }
  }
}
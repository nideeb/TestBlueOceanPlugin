pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
      }
    }

    stage('Test2') {
      parallel {
        stage('Test2') {
          steps {
            echo 'hi'
          }
        }

        stage('Test1') {
          steps {
            echo 'welcome'
          }
        }

      }
    }

    stage('Deloay') {
      steps {
        echo 'Deploy'
      }
    }

  }
}
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
        retry(count: 3)
        sh 'sdfghjlk'
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
        input(message: 'are you sure to deploay?', ok: 'yes i am sure')
      }
    }

    stage('Notify for new build') {
      steps {
        echo 'New build completed succesfuly'
      }
    }

  }
}
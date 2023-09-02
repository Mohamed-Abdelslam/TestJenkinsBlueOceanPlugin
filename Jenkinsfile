pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed.'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test1 Completed'
          }
        }

        stage('test1') {
          steps {
            echo 'Test1 Completed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy is Done Successfully!'
      }
    }

  }
}
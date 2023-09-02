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
            echo 'Test Completed'
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
        input(message: 'Are u sure u want to do this deploy?', ok: 'yes, i am sure')
      }
    }

    stage('Notify for New Build') {
      steps {
        echo 'New Build Completed Successfully.'
      }
    }

  }
}
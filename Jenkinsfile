pipeline {
  agent any
  stages {
    stage('Chrome') {
      parallel {
        stage('Chrome') {
          steps {
            echo 'Chrome Tests'
          }
        }

        stage('Firefox') {
          steps {
            echo 'Firefox Tests'
          }
        }

      }
    }

    stage('Edge') {
      steps {
        input(message: 'Do you want to continue?', ok: 'Continue')
        sleep 5
        echo 'Edge Tests'
      }
    }

  }
}
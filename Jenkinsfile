pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        echo 'Hello'
      }
    }

    stage('Stage 2.1') {
      parallel {
        stage('Step 2.1') {
          steps {
            sh 'echo \'Step 2.1\''
          }
        }

        stage('Stage 2.2') {
          steps {
            echo 'the step 2.2 parallel'
          }
        }

      }
    }

  }
}
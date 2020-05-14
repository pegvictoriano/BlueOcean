pipeline {
  agent any
  stages {
    stage('Fetch') {
      parallel {
        stage('Fetch') {
          steps {
            echo 'Test'
          }
        }

        stage('') {
          steps {
            git(url: 'https://github.com/pegvictoriano/BlueOcean', branch: 'master', changelog: true, credentialsId: 'pegvictoriano', poll: true)
          }
        }

      }
    }

    stage('Test') {
      steps {
        sleep 5
        echo 'Test Stage'
      }
    }

  }
}
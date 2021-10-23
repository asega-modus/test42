pipeline {
  agent any
  environment {
      IONIC_TOKEN = "un deux trois"
  }
  stages {
    stage('Running Tests') {
      steps {
         sh 'echo 42'
      }
    }

    stage('Building for platforms') {
      parallel {
        stage('Build Android') {
          steps {
	    sh 'echo 42'
          }
        }

        stage('Build iOS') {
          steps {
              sh 'echo Hello'
          }
        }

        stage('Build Live Update') {
          steps {
              sh 'echo 42'
          }
        }
      }
    }
  }
}

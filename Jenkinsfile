pipeline {
  agent any
  stages {
     steps {
        sh 'mvn --version '
      }
      post {
        success {
          echo "Now Archiving the Artufacts..."
          archiveArtifacts artifacts: '**/*'
        }
      }
     
    }
  }

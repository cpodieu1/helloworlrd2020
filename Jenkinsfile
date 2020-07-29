pipeline {
  agent any
  stages {
    stage('Buil Application') {
     steps {
        echo "welcome"
      }
      post {
        success {
          echo "Now Archiving the Artufacts..."
          archiveArtifacts artifacts: '**/*'
        }
      }
      
      }
     
    }
  }

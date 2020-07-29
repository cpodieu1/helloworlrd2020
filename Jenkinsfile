pipeline {
  agent any
  stages {
    stage('Buil Application') {
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
  }

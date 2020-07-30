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
      stage('Deploy in Staging Environment'){
        build job: 'Deploy_Application_Staging_Env'
      }
      
      }
     
    }
  }

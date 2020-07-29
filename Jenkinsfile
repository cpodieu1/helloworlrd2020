pipeline {
  agent any
   tools {
        M2_HOME 'apache-maven-3.6.3' 
   }
  stages {
    stage('Build Application') {
      steps {
        sh 'mvn --version '
      }
      post {
        success {
          echo "Now Archiving the Artufacts..."
          archiveArtifacts artifacts: '**/*.war'
        }
      }
    }
  }
}

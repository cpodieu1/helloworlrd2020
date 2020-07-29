pipeline {
  agent any
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

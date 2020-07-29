pipeline {
  agent any
  stages {
    stage('Build Application') {
      steps {
        sh 'mvn -f pom.xml clean package'
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

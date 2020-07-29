pipeline {
     agent any
     stages('Init') {
          steps {
               echo 'Hi, this is Podieu'
               echo 'We are Starging the Testing'
          }
     }
     stage('Build') {
          steps {
               echo 'Building Sample Maven project'
          }
     }
     stage('Deploy') {
          steps {
               echo "Deploying in Staging Area"
          }
     }
}

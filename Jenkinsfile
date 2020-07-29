pipeline {
     agent any
     stages {
          stage('Init') {
               steps {
                    echo 'Hi, this is Podieu'
                    echo 'We are Starting the Testing'
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
          stage('Deploy Production') {
          steps {
               echo "Deploying in production Area"
          }
          }
     }
}

     
         


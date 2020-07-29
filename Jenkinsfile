pipeline {
    agent any
    stages {
        stage('Init') {
            steps {
                echo 'hi this christ podieu'
                echo ' we are Starting the Testing'
            }
        }
        stage('Build') {
            steps {
                echo 'Building Sample Maven Project'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying in staging Area"
            }
        }
        stage('Deploy Production') {
            steps {
                echo "Deploying in Production Area"
            }
        }
    }
}
